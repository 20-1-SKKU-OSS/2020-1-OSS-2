---
title: 개인별 기여 내역 - 강성민
author: devquint
show_author_profile: true
tags: Role Python_Getting_Started
---

<div>{%- assign _detail = site.data.works.devquint-%}</div>

# {{ _detail.realnameKR }}

GitHub ID: {{ _detail.name }}

Name: {{ _detail.realnameKR }} ({{ _detail.realnameEN }})

## Works for team

<div>{%- include work-list.html userdata=_detail show_projects=false-%}</div>


## Works for project

<div>{%- include work-list.html userdata=_detail show_teams=false-%}</div>