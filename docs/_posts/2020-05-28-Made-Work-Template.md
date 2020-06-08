---
title: 개인별 역할 관련 템플릿 생성
author: devquint
show_author_profile: true
tags: Static_Page
---

# 작업 내역 정리 코드 생성

최종 프로젝트 정리를 위하여 개인별 기여 내역을 간단하게 확인할 수 있는 페이지를 만들어야 합니다.
메인, 포스트 등 다양한 페이지에서 확인할 수 있게끔 이를 별도의 코드와 y(a)ml 파일로 관리하도록 하였습니다.

## yml Schema 고안

[/data/works](https://github.com/20-1-SKKU-OSS/2020-1-OSS-2/tree/master/docs/_data/works) 내에 개인별로 yml 파일을 저장하는 것으로 하였습니다.

해당 파일에서 이름, id를 포함해 프로젝트 진행에 실제로 기여한 내용, 프로젝트 이외에 팀 활동을 위해 기여한 내용을 정리하도록 하였습니다. 
각 기여 활동에는 기여에 대한 설명과 Pull Request와 Issue 등 실제 웹 페이지 링크를 첨부하면 좋을 것이므로, 링크를 붙일 텍스트와 링크를 저장하여 표시할 수 있도록 했습니다. 
프로젝트 기여 활동에서는 개인별 기여 내용 요약 페이지를 정리할 시에 모든 기여내용을 저장할 수 없으므로 개인적으로 중요한 역할일 경우에 표시하여 요약 페이지에서 표시될지 여부를 선택할 수 있도록 했습니다.


실제 구조는 [Github에 올라온 예시 yml 파일](https://github.com/20-1-SKKU-OSS/2020-1-OSS-2/blob/master/docs/_data/works/example.yml)에서 확인할 수 있습니다.

## HTML & Jekyll Fluid 코드 제작

이제 이를 편하게 리스트로 볼 수 있도록 Jekyll Fluid를 활용하는 HTML 코드를 제작하였고 [/includes/work-list.html](https://github.com/20-1-SKKU-OSS/2020-1-OSS-2/blob/master/docs/_includes/work-list.html)에 저장하였습니다. 

기본적으로 userdata 인자로 특정 yml 파일을 인자로 받도록 하였습니다.
추가로 show_teams, show_projects, only_core의 boolean 인자를 받아 팀 활동 내역, 프로젝트 활동 내역, 요약본만 볼 것인지 여부를 확인할 수 있도록 했습니다.

코드 상에서는 전달받은 인자를 바탕으로 팀 활동 내역을 볼 것인지, 프로젝트 활동 내역을 볼 것인지, 주요 내용만 볼 것인지 등의 boolean값을 추가적으로 가져오고 `ul`을 활용해 리스트를 표시하도록 하였습니다.


# 사용방법

## 파일 지정

마크다운 코드 중 아래를 통해 yml파일을 지정해줍니다. assign할 변수 이름은 임의로 정하여도 상관없습니다.
아래의 경우 `_d1` 에 `example.yml` 을 불러옵니다.
```markdown 
<div>{% raw %}{%- assign _d1 = site.data.works.example-%}{% endraw %}</div>
```
<div>{%- assign _d1 = site.data.works.example-%}</div>

`example.yml`에 저장된 내용은 [Github 저장소 내부](https://github.com/20-1-SKKU-OSS/2020-1-OSS-2/blob/master/docs/_data/works/example.yml)를 확인해 주세요.


## 사용

이후 모든 기여 내역을 보는 것은 아래와 같이 합니다.
```markdown 
<div>{% raw %}{%- include work-list.html userdata=_d1 -%}{% endraw %}</div>
```


### 모두 보기

```markdown 
<div>{% raw %}{%- include work-list.html userdata=_d1 -%}{% endraw %}</div>
```

<div>{%- include work-list.html userdata=_d1 -%}</div>


### 핵심 기여 내용만 보기

```markdown 
<div>{% raw %}{%- include work-list.html userdata=_d1 only_core=true-%}{% endraw %}</div>
```

<div>{%- include work-list.html userdata=_d1 only_core=true -%}</div>


### 팀 기여 내용만 보기

```markdown 
<div>{% raw %}{%- include work-list.html userdata=_d1 show_projects=false-%}{% endraw %}</div>
```

<div>{%- include work-list.html userdata=_d1 show_projects=false-%}</div>


### 프로젝트 기여 내용만 보기

```markdown 
<div>{% raw %}{%- include work-list.html userdata=_d1 show_teams=false-%}{% endraw %}</div>
```

<div>{%- include work-list.html userdata=_d1 show_teams=false-%}</div>

### 주요 기여 내용 강조 해제

```markdown 
<div>{% raw %}{%- include work-list.html userdata=_d1 no_bold=true show_teams=false-%}{% endraw %}</div>
```

<div>{%- include work-list.html userdata=_d1 no_bold=true show_teams=false-%}</div>


# 실제 적용 예시

위의 경우 구분 없이 모든 리스트를 단순히 보여주기만 하므로 실제로 저대로 바로 사용하기에는 어려움이 있습니다.
따라서 적절히 변형하여 표시해줄 필요가 있습니다.

## 요약 페이지에서

요약 페이지는 본인이 핵심이라고 생각하는 작업내용만, id와 한글이름을 포함해 간단히 표시해줍니다.

```markdown 
<div>{% raw %}{%- assign _summary_example = site.data.works.example-%}{% endraw %}</div>

### {% raw %}{{ _summary_example.realnameKR }}{% endraw %} ({% raw %}{{ _summary_example.name }}{% endraw %})

<div>{% raw %}{%- include work-list.html userdata=_summary_example only_core=true-%}{% endraw %}</div>
```

<div>{%- assign _summary_example = site.data.works.example-%}</div>

### {{ _summary_example.realnameKR }} ({{ _summary_example.name }})

<div>{%- include work-list.html userdata=_summary_example only_core=true-%}</div>


## 상세 페이지에서

상세 페이지는 모두 보여주되 프로젝트 작업 내역과 팀 작업 내역을 구분해 보여줍니다.

```markdown 
<div>{% raw %}{%- assign _detail_example = site.data.works.example-%}{% endraw %}</div>

### {% raw %}{{ _detail_example.realnameKR }}{% endraw %}

GitHub ID: {% raw %}{{ _detail_example.name }}{% endraw %}

Real Name: {% raw %}{{ _detail_example.realnameKR }}{% endraw %} ({% raw %}{{ _detail_example.realnameEN }}{% endraw %})

#### Works for team

<div>{% raw %}{%- include work-list.html userdata=_detail_example show_projects=false-%}{% endraw %}</div>


#### Works for project

<div>{% raw %}{%- include work-list.html userdata=_detail_example show_teams=false-%}{% endraw %}</div>
```

<div>{%- assign _detail_example = site.data.works.example-%}</div>

### {{ _detail_example.realnameKR }}

GitHub ID: {{ _detail_example.name }}

Real Name: {{ _detail_example.realnameKR }} ({{ _detail_example.realnameEN }})

#### Works for team

<div>{%- include work-list.html userdata=_detail_example show_projects=false-%}</div>


#### Works for project

<div>{%- include work-list.html userdata=_detail_example show_teams=false-%}</div>