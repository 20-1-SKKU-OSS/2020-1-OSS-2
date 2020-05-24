---
title: python_getting_started 프로젝트 개인별 역할 분담
author: devquint
show_author_profile: true
mathjax: false
mathjax_autoNumber: false
tags: Python_Getting_Started Pre_Investigation Role
---

# 개인별 역할 분담

선호에 따라서 원하는 내용을 진행하기로 하였습니다. 이 내용은 초안이며, 추후 프로젝트 진행에 따라 달라질 수 있습니다.

오픈소스소프트웨어의 특성상 다른 커뮤니티 기여자가 발생하는 등 일정이 변동되기 쉽기 때문에 개략적인 작업 순서만 정하였습니다.
작업 순서는 아래 개인별 역할 분담에 서술된 순서이며, 코드 리뷰는 상시 진행합니다.
상술한 대로 이 포스트는 초안이며, 일정은 추후 변경될 수 있습니다.

팀장 우선, 이후 가나다 순으로 작성하였습니다.


## 강성민 `팀장`{:.info}

<div>{%- assign _a1 = site.data.authors["devquint"] -%}</div>
<div>{%- include article/footer/author-profile.html author=_a1 -%}</div>

- `python-for-beginners`의 01번 항목을 문서로 작성
- `python-for-beginners`에 관한 커밋들의 동료 코드 리뷰 진행
- `more-python-for-beginners`의 코드 검토, 주석 및 코드의 오타 검수
- `even-more-python-for-beginners-data-tools`의 문서 및 코드를 읽고 이해하기 어렵거나 코드에 기본적인 문제가 있는 부분에 대한 Issue 작성
- `more-python-for-beginners`의 주요 문서 한글 번역 진행


## 김도열

<div>{%- assign _a2 = site.data.authors["Dorika0203"] -%}</div>
<div>{%- include article/footer/author-profile.html author=_a2 -%}</div>

- Issue 중 Pull Request가 없는 issue `#3`, `#6`에 대해 해결하여 Pull Request
- `more-python-for-beginners`의 이해하기 힘들거나 어려운 부분에 대해 Issue 작성
- `more-python-for-beginners`의 코드 내용 검증
- `more-python-for-beginners`의 오류 발견 및 수정
- `more-python-for-beginners`의 문서 부연 설명, 코드 내 주석 작성



## 서채연

<div>{%- assign _a3 = site.data.authors["ChaeyeonSeo"] -%}</div>
<div>{%- include article/footer/author-profile.html author=_a3 -%}</div>

- `python-for-beginners`의 코드 리뷰
- `python-for-beginners`의 오류 발견 및 수정
- `python-for-beginners`의 초보자 입장에서 이해하기 힘든 부분에 대한 설명 작성 및 필요한 코드 추가
- `python-for-beginners`의 주요 문서 한글 번역



## 이종윤

<div>{%- assign _a4 = site.data.authors["jesusleejy"] -%}</div>
<div>{%- include article/footer/author-profile.html author=_a4 -%}</div>

- python-for-beginners에서 추가할 만한 python 기초 설명 코드 추가
- python-for-beginners의 기존 콘텐츠를 보다 이해하기 쉽도록 코드 및 주석 정리
- python-for-beginners의 Slides 폴더 내의 ppt 개선 작업
- python-for-beginners의 Slides 폴더 내의 ppt 한글 번역



## 정현태

<div>{%- assign _a5 = site.data.authors["Hyuntae-Jeong"] -%}</div>
<div>{%- include article/footer/author-profile.html author=_a5 -%}</div>

* `python-for-beginners`의 Slides 폴더 내의 문서 Leading Zero 추가 
* `python-for-beginners`의 모든 README.md에 대하여
	* 초보자 관점에서의 추가 영어 및 한글 부가설명 작성 (번역은 후순위)
	* 적합한 Programming Concept에 대한 정보 추가
* `python-for-beginners`의 코드들에 대해서 직관적인 설명이 필요한 부분을 찾아 주석 추가 작성 및 이해에 도움이 될 정보 추가
* 전체적인 내용에 대해, 직접 코드를 실행하고 확인하면서 문제 발생 가능성에 대한 검토
