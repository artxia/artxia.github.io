---
layout: markdown_page
title: Working with Trial Extensions
category: License and subscription
---

### On this page
{:.no_toc}

- TOC
{:toc}

----

## Overview

Use these workflows if you need to extend a GitLab trial.


## Extending GitLab.com Trials
### Downgrading a Trial (console access required)
From time-to-time a prospect will not want to trial Gold, but rather the features available at another tier.
In these cases, you'll need to downgrade the trial.

To do so, you'll need console access on customers.gitlab.com.

Use one of these methods to perform the downgrade.
```
def downgrade_trial_to_silver(group_id)
  order = Order.find_by_gl_namespace_id group_id
  return "Unable to find Order with that group_id" unless order
  order.update_attributes!(gl_namespace_id: nil, product_rate_plan_id: Plan::SILVER_PLAN, trial: true)
  # we need to set namespace_id again given the sync service only calls GL.com API if it has changed.
  order.update_attributes!(gl_namespace_id: group_id)
  Gitlab::Namespace::UpdatePlanInfoService.new(order).execute
end

def downgrade_trial_to_bronze(group_id)
  order = Order.find_by_gl_namespace_id group_id
  return "Unable to find Order with that group_id" unless order
  order.update_attributes!(gl_namespace_id: nil, product_rate_plan_id: Plan::BRONZE_PLAN, trial: true)
  # we need to set namespace_id again given the sync service only calls GL.com API if it has changed.
  order.update_attributes!(gl_namespace_id: group_id)
  Gitlab::Namespace::UpdatePlanInfoService.new(order).execute
end
```

### Extending a trial that hasn't expired
#### From customers.gitlab.com
1. Identify the customer in the [customers portal](https://customers.gitlab.com)
1. From the GitLab Groups tab change the `Exp on:` date:

#### From the rails console
Use this method to peform the extension
```
def extend_trial(group_id, date)
  order = Order.find_by_gl_namespace_id group_id
  return "Unable to find Order with that group_id" unless order
  order.update_attributes!(gl_namespace_id: nil, product_rate_plan_id: Plan::GOLD_PLAN, end_date: Date.parse(date), trial: true)
  # we need to set namespace_id again given the sync service only calls GL.com API if it has changed.
  order.update_attributes!(gl_namespace_id: group_id)
  Gitlab::Namespace::UpdatePlanInfoService.new(order).execute
end
```

### Extend a trial that has expired (console access required)
Use the `extend_trial` method defined above.
 

## Extending GitLab Self-managed Trials
Self-managed trials cannot be extended -  a license must be re-issued and applied to the instance in order to "extend" a trial.
Self-managed licesnses are managed in the [license app](https://license.gitlab.com). In order to sign-in, you will need an account on `dev.gitlab.org`. If you don't have one, please speak with your manager to arrange access.

To re-issue a license:
1. Log in to the [license app](https://license.gitlab.com)
1. Identify the trial license by searching by customer or company name.
1. Click the name on the license to view its details.
1. In the **Edit license** section, choose _Duplicate license_
1. Modify the `Users count` and `Expires at` fields, consider adding a note to describe why you're issuing this license.
1. Click **Create license**

The license should be emailed out immediately, but you're also welcome to download it and pass it along to the customer directly.
