---
title: "[북클럽 리뷰] Clean Architecture - ch1"
excerpt: "인트로, 1장 - 설계와 아키텍쳐란"

categories:
  - review
tags:
  - [bookclub, clean architecture, book review]

toc: true
toc_sticky: true
 
date: 2021-08-05
last_modified_at: 2021-08-05
---

## Intro
회사에서 매주 목요일 북클럽을 진행한다.  
몇 달간 `실용주의 프로그래머`로 진행했고, 이번 주부터는 `클린 아키텍처`라는 책으로 진행된다.  
`클린 아키텍처`는 개발팀 내에서 책을 추천해서 다수결로 선정되었다.  
[**Robert C. Martin의 Clean Architecture**]

매주 2개의 챕터를 읽고 토론하는 방식으로 진행되는데, 가끔 대충 좀 흘려듣기도 하고 그런 게 조금 아까워서 시간이 날 때 조금씩 그 주에 한 북클럽 내용을 정리해 보려고 한다.  
뭐 겸사겸사 영어 단어도 정리하고...  

회사에선 물론 원서로 진행해서 아마존에서 구매했다. 혹시나 해서 YES24를 보니 ebook이 있길래 한글 버전도 샀다. 
아직 책을 다 본 게 아니라서 원서와 한국어 버전이 얼마나 다른지 모르겠지만 일단 1부 소개와 1부-1장은 똑같았다.

자세한 내용을 적는 건 책을 낸 분들의 노력을 무시하는 것 같아서 대충 어떤 내용으로 북클럽이 진행되었는지와 함께 공유했던 내용을 적어보려고 한다.

## Introduction
저자는 제대로 된 소프트웨어를 만들면 어떤 이점이 있는지 간단하게 설명한다.
- 적은 인력으로 새로운 기능을 추가, 유지보수
- 빠르고 단순한 변경
- 낮은 결함률
- 최소한의 노력으로 기능, 유연성 등을 극대화

원서에서 이를 유토피아라고 하면서 실제로 저자는 그런 아키텍처 환경에서 일해 보았다고 한다.
그러면서 그 반대의 경우에서의 경험을 묻는다.

이번 북클럽 진행은 내가 했는데, 1부 소개에서 우리는 형편없는 소프트웨어 설계 속에서 일했던 경험을 공유했다.

## Chapter1 - 설계와 아키텍처란?
저자는 좋은 소프트웨어 설계의 목표를 아래와 같이 정의한다.
> 소프트웨어 아키텍처의 목표는 필요한 시스템을 만들고 유지보수 하는 데 투입되는 인력을 최소화하는 데 있다.

아, 문득 이런 생각이 든다. 투입되는 인력이 최소화되어서 우리 회사가 더는 날 필요로 하지 않으면 어쩌지....😂

저자는 이를 뒷받침하는 여러 차트를 보여주는데 꽤 흥미로웠다.  
그래프와 설명이 모두 보고 이해하기 쉬웠다. TDD에 관한 그래프도 있었는데, 우리 회사 엔지니어 매니저가 항상 TDD를 강조하셔서 조금 더 흥미롭게 느껴졌다.

당연하지만 기본적인 프로그래머의 자세에 대해 다시 한번 생각해 볼 수 있는 챕터였다.

우리는 무엇이 좋은 아키텍처의 조건인지, 그리고 훌륭한 아키텍처를 만들기 위해서 우리가 할 수 있는 일은 무엇인지에 관해서 토론하였다. 오늘 북클럽을 하면서 같이 일하는 개발자들이 무엇을 중시하는지 조금 더 이해할 수 있었다.

아, 이 책이 끝나는 날. 우리의 생각이 얼마나 바뀌었는지도 이야기해보기로 했다.

