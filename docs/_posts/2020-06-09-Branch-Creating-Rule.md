---
title: 팀 프로젝트 branch 구분계획
author: Dorika0203  
show_author_profile: true
tags: Python_Getting_Started
---

### 브랜치 구분 계획

#### 레벨별 폴더에 따른 상위 브랜치 3개


현재 프로젝트에는 초급자, 중급자, 고급자용으로 공부할 단원에 대한 코드들이 3개의 폴더로 나누어져 정리되어 있다.<br/>폴더명은 각각 python-for-beginners, more-python-for-beginners, even-more-python-for-beginners 이다.<br/>프로젝트를 진행하면서, 우리 팀은 이 폴더들을 pfb, mpfb, empb로 줄여서 부르기도 했다.

각각의 폴더에 대해 개선할 3개의 브랜치는 다음과 같다.

- better-python-for-beginners
- better-more-python-for-beginners
- better-even-more-python-for-beginners

#### 단원별 브랜치 생성

위에서 소개한 pfb, mpfb, empb 브랜치에서, 폴더에 있는 각각의 단원들에 대한 수정을 진행하는 브랜치 생성 방법은 다음과 같다.

##### 예시 1: more-python-for-beginners의 02 - Lambdas(2단원)을 수정하는 경우

    + better-more-python-for-beginners에서 분기하는 브랜치 better-more-02를 생성
    
    + (로컬에서) git checkout -b better-more-02 origin/better-more-python-for-beginners
    
    
    
##### 예시 2: python-for-beginners의 09 - Handling multiple conditions(9단원)을 수정하는 경우

    + better-python-for-beginners에서 분기하는 브랜치 better-09를 생성
    
    + (로컬에서) git checkout -b better-09 origin/better-python-for-beginners
  
