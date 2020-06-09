---
title: 팀 프로젝트의 Pull Request와 Code review 
author: jesusleejy 
show_author_profile: true
tags: Python_Getting_Started Work_Process
---

Pull Request와 Code review 진행 상황
======================================

[1] Pull Request 진행 상황(Merge된 PR 기준)
----------------------------------------

-Comment 수정에 관한 Pull Request  
[reorder-comment-Sort-alphabetically](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/1)  
[[UPDATE] fix comment of method_sorter.py](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/23)  
[Fix a typing error of comments in pfb1-10](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/49)  
[Fix a typing error of comments in pfb11-18](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/53)  
[Fix errors in comments in mpfb 1-9](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/52)

-Comment 추가에 관한 Pull Request  
[Add coment 1](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/5)  
[[UPDATE]Add comment](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/14)

-README 수정에 관한 Pull Request  
[[FIX]fix a typing error](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/13)  
[Fast-forward project](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/17)

-File Name 수정에 관한 Pull Request  
[[UPDATE]Fix file name](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/3)  
[[UPDATE]Changed all folder name Slides to 00 - Slides](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/12)  
[[Update] Changed folder name 'Slides' to '00 - Slides' in python-for-beginners](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/18)  
[Revert "[UPDATE] Changed all folder name Slides to 00 - Slides"](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/16)  
[[UPDATE]Changed folder name "Slides" to "00 - Slides" in better-more-python-for-beginners](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/47)

-개별 py파일 내용 수정 및 추가에 관한 Pull Request  
[Fix code challenge solution.py](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/4)  
[Fix method_sorter.py in more-python/chapter 2](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/7)  
[[ADD]add simple example using decorator](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/8)  
[Added more details to decorators_simple.py](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/24)

-Unifying Indentation에 관한 Pull Request  
[Unifying indentation: python-for-beginners/chapter 2-4](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/28)  
[Unifying indentation: python-for-beginners/chapter 5-7](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/51)  
[Unifying indentation: python-for-beginners/chapter 8-10](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/31)  
[Unifying indentation: python-for-beginners/chapter 11-13](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/39)  
[Unifying indentation: python-for-beginners/chapter 14-16](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/41)  
[Unifying indentation: python-for-beginners/chapter 17-18](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/43)  
[Unifying indentation: more-python-for-beginners/chapter 1-3](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/30)  
[Unifying indentation: more-python-for-beginners/chapter 4-6](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/33)  
[Unifying indentation: more-python-for-beginners/chapter 7-9](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/36)  
[Unifying indentation: even-more-python-for-beginners-... chapter 1-5](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/22)  
[Unifying indentation: even-more-python-for-beginners/chapter 6-10](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/46)  
[Unifying indentation: even-more-python-for-beginners-... chapter 11-15](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/48)  
[Indent unify of python-for-beginners](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/54)  
[Indent unify of more-python-for-beginners](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/55)  
[Indent unify of even-more-python-for-beginners-data-tools](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/56)

[2] Code review 진행 상황
----------------------------------------

c9-python-getting-started는 파이썬에 관한 내용을 알려주는 가이드북이기 때문에, 
대부분의 Code Review들은 수정 및 추가된 code와 comment의 문법적 오류와 가독성을 개선하는 방향으로 이루어졌다.
13주차 Code Review 강의 내 Rule of Code Review의 내용에서 컨벤션(코드스타일) 지적은 피하자는 부분이 있지만,
본 프로젝트는 가이드북 프로젝트이고 [PEP8](https://www.python.org/dev/peps/pep-0008/)도 소개하고 있기 때문에 컨벤션 지적도 함께 이루어졌다.

-예시
1. [Comment 추가에 관한 Pull Request](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/5)  
2. [가독성 개선에 관한 Code Review](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/5#pullrequestreview-421394463)  
3. [Commit 1차 수정](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/5/commits/c47e8a63cecf5b4b6bce5c174f82121a16667dc4)  
4. [Convention 지적에 관한 Code Review](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/5#pullrequestreview-421482094)  
5. [Commit 2차 수정](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/5/commits/87fcdccb86f312388d1dc320198fcacf9b7f7236)

위와 같은 방식으로 Code Review와 수정이 이루어졌다.

