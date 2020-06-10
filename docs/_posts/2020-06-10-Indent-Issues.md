---
title: Indent 관련 Issue 정리
author: Hyuntae-Jeong
show_author_profile: true
tags: Python_Getting_Started Indent_Issues
---

Indent 관련 Issue 정리 및 개선 사항
======================================

[1] Indent 관련 Issue 문제 제기
----------------------------------------

- Found Problem Not Working, Question about Formatting  
[Fix codes in more-python/chapter 1 #6](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/6)
- Found Reason of the problem Not Working, Confusion with Spaces and Tabs  
[Fix good.py #9](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/9)
- New issue started about PEP 8's 4 spaces
[Comment on PR #9](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/9#pullrequestreview-421493633)
- Unified indents to tab
[Unify indents to tab #10](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/pull/10)
- New issue opened about Indentation Consistency
[Indentation Consistency Issue #11](https://github.com/20-1-SKKU-OSS/c9-python-getting-started/issues/11)




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
