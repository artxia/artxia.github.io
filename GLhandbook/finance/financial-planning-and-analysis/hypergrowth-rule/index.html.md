---
layout: handbook-page-toc
title: "The Hypergrowth Rule"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}


## The Hypergrowth Rule

GitLab aspires to using The Hypergrowth Rule by [November 18, 2023](/company/strategy/#sequence). Until that time as a percent of revenue, we are spending at a higher rate in all groups (except G&A and cost of sales) compared to companies at similar stages of growth. We do this to advance the product, increase our TAM, and increase market share through a new [channel strategy](/handbook/sales/channel/). We believe this investment will result in higher growth rates compared to similar companies.

### Rule of 40  

The hypergrowth rule is a standard for measuring and thinking about profitability at any growth rate.
It's inspired, in part, by the [Rule of 40](https://feld.com/archives/2015/02/rule-40-healthy-saas-company.html), a SaaS rubric for growth that `Revenue Growth % + Free Cash Flow % = 40`.
There is a high correlation between level of attainment of this combined metric and company valuation - although data suggests that current investor valuations models are more highly correlated with revenue growth rate.

### Importance

We believe that strong correlation is a result of the importance of capturing market share.
Using the Rule of 40 as an example, when Revenue growth is greater than 40%, there is an implication that negative profitability is encouraged, but this fails to answer key questions, such as:
* How much should I be investing in different parts of the business?
* How much should I be willing to lose today?
* As growth slows because of market dominance, what is the path to profitability?

The below hypergrowth rule can help answer the questions that the Rule of 40 doesn't answer.

### Rule of 50

We also believe that with our efficient business model that leverages a strong installed base of open source users and community contributions that we should achieve our long term profitability targets when our growth drops to 30%. In other words we have adopted a Rule of 50 approach instead of the [Rule of 40](#rule-of-40) to how we think about the trade-off between growth and profitability.

Our model target is our [long term profitability target](/handbook/finance/financial-planning-and-analysis/#long-term-profitability-targets).

### Formula

`Division expense target = ((Revenue Delta * Growth Lever ) * Model Percent ) + Model Percent)`

#### Division Expense Targets

Division Expense Targets are the optimal percent of revenue for each functional group in a given period, this is the output of this formula.

#### Revenue Delta

Revenue Delta is the difference between Revenue Growth and Eventual Profit Margin. For GitLab the Eventual Profit Margin is 20% because our [target costs are 80%](/handbook/finance/financial-planning-and-analysis/#long-term-profitability-targets). 

#### Growth Lever

The growth lever is equal to `1 / (sum of target divisional % of revenue for divisions that should be variable based on growth)`.
For GitLab, it is: `1 / (Sales + R&D + G&A + Marketing % of Rev)`, which would equal 1.25, but because cost of sales and hosting don’t increase with faster revenue growth, we can remove those (17%), and what's left is `1/(80%-17%)` which ~ 1.5.
This makes the full formula for the growth lever: `1 / (Sales + R&D + G&A + Marketing % of Rev - Variable Non-Delayed Costs)`.

The growth lever is equal to 1.5.

#### Model Percent

Our model percent is our [long term profitability target](/handbook/finance/financial-planning-and-analysis/#long-term-profitability-targets) for each division.

### Example of the Hypergrowth Formula

Below is an **illustrative** example, using the hypothetical case of revenue growth being 150%:

| Factor | Formula|
|--------|--------|
|Revenue growth | 150% |
|Revenue growth - 20% | 130% = 1.3 |
|(Revenue growth - 20%) * 1.5| 1.3 * 1.5  = 1.95 |
|((Revenue growth - 20%) * 1.5 ) * model % )| 1.95*0.23=0.4485 |
|((Revenue growth - 20%) * 1.5 ) * model % ) + model %|0.4485+0.23=0.6785|
|Optimal % of revenue for a division|0.6785 = 67.85%|
