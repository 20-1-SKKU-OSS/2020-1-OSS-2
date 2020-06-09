---
title: 개인별 기여 내역 - 이종윤 
author:
show_author_profile: true
tags: Role Python_Getting_Started
---

<div>{%- assign _detail = site.data.works.example -%}</div>

# {{ _detail.realnameKR }}

<div>{%- assign _a1 = site.data.authors["jesusleejy"] -%}</div>
<div>{%- include article/footer/author-profile.html author=_a1 -%}</div>

## Works for team

<div>{%- include work-list.html userdata=_detail show_projects=false-%}</div>


## Works for project

<div>{%- include work-list.html userdata=_detail show_teams=false-%}</div>