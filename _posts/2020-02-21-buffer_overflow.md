---
layout: post
title:  "버퍼 오버플로우"
date:   2021-02-21 14:23:13
author: John Choi
sitemap:
categories: 보안
---

# 버퍼 오버플로우
####  1. 스택 오버플로우 (Stack Overflow)
- 스택에 할당된 버퍼들이 문자열 계산 등에 의해 정의된 버퍼의 한계치를 넘는 경우

#### 2. 힙 버퍼 오버플로우 (Heap Buffer Overflow)
-  최초 정의된 힙의 메모리 사이즈를 초과할 때.

#### 3. 스택 오버플로우의 방지
- strncpy를 통해 방지한다.
- 스택 가드 : 복귀 주소의 특정 값을 저장하여, 변경시 공격으로 간주
- 스택 쉴드 : 복귀 주소를 특수 스택에 저장
- ASLR (**Address Space Layout Randomization**) : 주소 배치의 난수화, 실행 시마다 메모리 주소를 변경시켜 악성 코드에 의한 특정 주소 호출을 방지


