---
layout: handbook-page-toc
title: "Baseline Entitlement System Flow"
---

<div class="center">
<div style="width: 640px; height: 480px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:640px; height:480px" src="https://www.lucidchart.com/documents/embeddedchart/0b61de33-78e1-4690-ac62-73e6d13c64b8" id="kiComslljY4L"></iframe></div>
</div>


##### gitlab-services

`gitlab-services` hosts GitLab apps such as `version`, `license`, `forum`, etc.

All members of the group `gitlab-org` are provided `reporter` access to `gitlab-services` as the group `gitlab-org` was granted that role within `gitlab-services`.

This allows all GitLab team members to access and submit issues while removing the ability for non-engineers to push to production.
Access Requests may be opened to request a higher role in `gitlab-services`.
