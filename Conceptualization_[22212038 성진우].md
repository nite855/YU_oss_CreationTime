# 1. Conceptualization

## Project Title
Creation Time

## Student Info
- Student No: 
- Name: 성진우
- E-mail: 

---

## Revision History

| Revision date | Version # | Description | Author |
|--------------|----------|------------|--------|
| 2026.03.22 | 1.0.0 | first draft | 성진우 |

---

## Contents
1. Business purpose  
2. System context diagram  
3. Use case list  
4. Concept of operation  
5. Problem statement  
6. Glossary  
7. References  

---

# 1. Business Purpose

‘인간은 사회적 동물이다’라는 아리스토텔레스의 말처럼 인간은 타인과 관계를 맺고 공동체를 이루며 살아가는 존재이다.  

현대사회에서 사람들은 가족, 친구, 직장 등 다양한 관계 속에서 살아가며, 최근에는 바쁜 일상 속에서도 취미 기반의 소모임을 통해 스트레스를 해소하려는 경향이 증가하고 있다. 특히 ‘감자튀김 모임’과 같은 새로운 형태의 소모임 문화는 짧고 부담 없는 만남을 통해 2030 세대에게 큰 관심을 받고 있다.  

이러한 흐름에 따라 취향 공유 플랫폼 또한 빠르게 성장하고 있다. 대표적으로 당근마켓은 지역 기반 커뮤니티로 확장하며 ‘모임’ 기능을 도입하였고, 출시 1년 만에 이용자 수 1500만 명을 돌파하였다.  

그러나 대학 환경에서는 팀 프로젝트가 단순한 취미를 넘어 평가와 직결되며, 높은 피로도를 유발한다. 특히 팀원 모집과 일정 조율이 큰 부담으로 작용한다.  

이러한 문제를 해결하기 위해 **대학생 대상 팀원 매칭 및 팀 운영 플랫폼 ‘Creation Time’**을 개발한다.  

### 목표
- 효율적인 팀원 모집
- 원활한 팀 운영

---

# 2. System Context Diagram

## 기능 목록

| 기능 | 설명 |
|------|------|
| SignUp | 회원가입 |
| Login | 로그인 |
| CreateTeam | 팀 만들기 |
| CreateRecruitPost | 모집글 작성 |
| ApplyTeam | 팀 지원 |
| ReviewApplication | 팀 승인/거절 |
| ManageTeam | 팀원 관리 |
| CreateVote | 투표 생성 |
| ParticipateVote | 투표 참여 |
| ViewVoteResult | 투표 결과 확인 |
| CreateSchedule | 일정 등록 |
| WritePost | 게시글 작성 |
| ReadPost | 게시글 확인 |
| ExportData | 엑셀로 데이터 내보내기 |

---

# 3. Use Case List

> User는 Member와 TeamLeader로 구분된다.

## Use Case Table

| Use Case | Actor | Description |
|----------|------|-------------|
| SignUp | Member | 회원가입 수행, 기본 정보 및 기술 스택 입력 |
| Login | Member, TeamLeader | 계정 인증 후 로그인 |
| CreateTeam | Member | 팀 생성 및 TeamLeader 권한 획득 |
| CreateRecruitPost | TeamLeader | 팀원 모집글 작성 |
| ApplyTeam | Member | 팀 지원 |
| ReviewApplication | TeamLeader | 지원자 승인/거절 |
| ManageTeam | TeamLeader | 팀원 관리 |
| CreateVote | TeamLeader | 투표 생성 |
| ParticipateVote | Member | 투표 참여 |
| ViewVoteResult | Member, TeamLeader | 투표 결과 확인 |
| CreateSchedule | TeamLeader | 일정 등록 |
| WritePost | Member, TeamLeader | 게시글 작성 |
| ReadPost | Member, TeamLeader | 게시글 확인 |
| ExportData | TeamLeader | CSV 데이터 다운로드 |

---

# 4. Concept of Operation

## 1) SignUp

| 항목 | 내용 |
|------|------|
| Purpose | 사용자 계정 생성 |
| Approach | 기본 정보 입력 후 DB 저장 |
| Dynamics | 회원가입 요청 시 |
| Goals | 계정 생성 및 정보 저장 |

---

## 2) Login

| 항목 | 내용 |
|------|------|
| Purpose | 사용자 인증 |
| Approach | ID/비밀번호 검증 |
| Dynamics | 로그인 요청 시 |
| Goals | 권한 획득 |

---

## 3) CreateTeam

| 항목 | 내용 |
|------|------|
| Purpose | 팀 생성 |
| Approach | 팀 정보 입력 후 DB 저장 |
| Dynamics | 팀 생성 요청 시 |
| Goals | TeamLeader 권한 획득 |

---

## 4) CreateRecruitPost

| 항목 | 내용 |
|------|------|
| Purpose | 모집글 작성 |
| Approach | 모집 정보 입력 |
| Dynamics | 팀 생성 이후 |
| Goals | 팀원 모집 가능 |

---

## 5) ApplyTeam

| 항목 | 내용 |
|------|------|
| Purpose | 팀 지원 |
| Approach | 모집글에서 지원 |
| Dynamics | 지원 버튼 클릭 |
| Goals | 지원자 목록 등록 |

---

## 6) ReviewApplication

| 항목 | 내용 |
|------|------|
| Purpose | 지원자 승인/거절 |
| Approach | 지원자 정보 확인 후 처리 |
| Dynamics | 지원 목록 조회 시 |
| Goals | 팀원 확정 |

---

## 7) ManageTeam

| 항목 | 내용 |
|------|------|
| Purpose | 팀 관리 |
| Approach | 팀원 변경 및 역할 부여 |
| Dynamics | 관리 요청 시 |
| Goals | 팀 구성 유지 |

---

## 8) CreateVote

| 항목 | 내용 |
|------|------|
| Purpose | 투표 생성 |
| Approach | 투표 항목 입력 |
| Dynamics | 투표 생성 시 |
| Goals | 의사결정 지원 |

---

## 9) ParticipateVote

| 항목 | 내용 |
|------|------|
| Purpose | 투표 참여 |
| Approach | 투표 선택 |
| Dynamics | 참여 시 |
| Goals | 결과 반영 |

---

## 10) ViewVoteResult

| 항목 | 내용 |
|------|------|
| Purpose | 투표 결과 확인 |
| Approach | 결과 조회 |
| Dynamics | 조회 시 |
| Goals | 결과 확인 |

---

## 11) CreateSchedule

| 항목 | 내용 |
|------|------|
| Purpose | 일정 등록 |
| Approach | 캘린더 입력 |
| Dynamics | 일정 추가 시 |
| Goals | 일정 공유 |

---

## 12) WritePost

| 항목 | 내용 |
|------|------|
| Purpose | 게시글 작성 |
| Approach | 글 작성 후 저장 |
| Dynamics | 작성 시 |
| Goals | 정보 공유 |

---

## 13) ReadPost

| 항목 | 내용 |
|------|------|
| Purpose | 게시글 확인 |
| Approach | 게시글 조회 |
| Dynamics | 선택 시 |
| Goals | 의사소통 |

---

## 14) ExportData

| 항목 | 내용 |
|------|------|
| Purpose | 데이터 다운로드 |
| Approach | CSV 생성 |
| Dynamics | 다운로드 요청 시 |
| Goals | 외부 활용 |

---

# 5. Problem Statement

## Overview
Creation Time은 팀원 매칭 및 일정 관리 웹 플랫폼이다.

## Problems

### Problem #1 – 직관적인 인터페이스
- 정보 과다로 인해 UX 저하 가능

### Problem #2 – 다양한 디바이스
- 모바일/PC 환경 대응 필요

### Problem #3 – 모임 구분
- 다양한 팀 유형 분류 필요

### Problem #4 – 데이터 무결성
- 동시 요청 시 데이터 충돌 가능

### Problem #5 – 권한 관리
- 역할 기반 접근 제어 필요

### Problem #6 – 동시 접속
- 다수 사용자 처리 필요

---

## NFRs

1. 데이터 정확성 및 일관성 보장  
2. 직관적인 UI 제공  
3. 안정적인 성능 유지  
4. 동시 접속 안정성 확보  

---

# 6. Glossary

| 용어 | 설명 |
|------|------|
| Team | 프로젝트 수행 단위 |
| Recruit Post | 팀원 모집글 |
| User | Member + TeamLeader |
| Application | 팀 지원 정보 |
| Vote | 의사결정 투표 |

---

# 7. References

- https://topclass.chosun.com/news/articleView.html?idxno=35975  
- https://v.daum.net/v/0XJXDMB3lx?f=p  
- https://news.gknu.ac.kr/news/articleView.html?idxno=1802  
- https://www.asiatime.co.kr/article/20251105500311  
