---
title: 팀 프로젝트 branch 구분계획
author: Dorika0203  
show_author_profile: true
tags: Python_Getting_Started
---

### 브랜치 구분 계획

#### 레벨별 폴더에 따른 상위 브랜치 3개


현재 프로젝트에는 초급자, 중급자, 고급자용으로 공부할 단원에 대한 코드들이 3개의 폴더로 나누어져 정리되어 있습니다.<br/>폴더명은 각각 python-for-beginners, more-python-for-beginners, even-more-python-for-beginners 입니다.<br/>저희 팀은 프로젝트를 진행하면서, 이 폴더들을 pfb, mpfb, empfb로 줄여서 부르기로 했습니다.

각각의 폴더에 대해 개선할 3개의 브랜치는 다음과 같습니다.

- better-python-for-beginners
- better-more-python-for-beginners
- better-even-more-python-for-beginners


#### 단원별 브랜치 생성

위에서 소개한 pfb, mpfb, empfb 브랜치에서, 폴더에 있는 각각의 단원들에 대한 수정을 진행하는 브랜치 생성 규칙은 다음과 같습니다.

##### 예시 1: more-python-for-beginners의 02 - Lambdas(2단원)을 수정하는 경우

    better-more-python-for-beginners에서 분기하는 브랜치 better-more-02를 생성
    
    (로컬에서) git checkout -b better-more-02 origin/better-more-python-for-beginners
    
    
    
##### 예시 2: python-for-beginners의 09 - Handling multiple conditions(9단원)을 수정하는 경우

    better-python-for-beginners에서 분기하는 브랜치 better-09를 생성
    
    (로컬에서) git checkout -b better-09 origin/better-python-for-beginners
    
#### 예외 경우 - indent unifying issue

코드 수정을 하던 중 저희는 프로젝트 전반에 걸쳐 indent와 관련된 코드 에러가 빈번함을 발견했습니다.<br/>
[초기에 생성되었던 Issue](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/issues/11)<br/>
[1차 합의점 달성 및 브랜치 생성 논의](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/issues/15)<br/>
[최종 Issue - indentation 수정 방법 공지 및 역할분담](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/issues/20)<br/>

Issue를 통해 팀원들 간 전체적인 project에서 어떻게 indentation을 수정할지 논의했습니다.<br/>
그 과정에서 결정된 브랜체 생성 규칙은 다음과 같습니다.

1. 3개의 폴더에 따른 indent 수정용 브랜치를 생성

- indent-pfb
- indent-mpfb
- indent-empfb

2. 자신이 수정할 부분에 대한 Issue를 생성한다. 예시 : more-python-for-beginners의 1~3단원의 indent를 수정하고자 하는 경우

``` 
Issue 제목: Unifying indentation: more-python-for-beginners chatper 1-3
    
[링크](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/issues/26)
```

3. 해당 이슈 번호 (위의 예시의 경우는 26번임)를 기반으로 브랜치를 생성한다.

```
    새로 만들어질 브랜치 명: Issue-26
    
    분기할 브랜치: more-python-for-beginners의 단원들을 수정하므로 indent-mpfb를 분기할 브랜치로 선택
    
    (로컬에서) git checkout -b Issue-26 origin/indent-mpfb
```   
    
