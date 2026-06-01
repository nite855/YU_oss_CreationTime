# 1. Conceptualization

## Project Title
Creation Time

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/495abca5-12ba-4492-b353-d19c9a71695a" />

## Student Info
- Student No: 22212038
- Name: 성진우
- E-mail: wlsdn4271@naver.com

---

## Revision History

| Revision date | Version # | Description | Author |
|--------------|----------|------------|--------|
| 2026.03.25 | 1.0.0 | first draft | 성진우 |
| 2026.04.28 | 1.1.0 | use case 수정 및 오타 수정, 패널티 점수 추가 | 성진우 |
| 2026.04.29 | 1.2.0 | Actor 재정의 | 성진우 |
| 2026.05.01 | 1.3.0 | use case 수정 및 삭제, 수정 use case 추가 | 성진우 |
| 2026.05.03 | 1.4.0 | use case 수정 | 성진우 |
| 2026.05.14 | 1.5.0 | Viewing Schedule 추가 | 성진우 |  
| 2026.05.20 | 1.6.0 | Starting Recruitment, Closing Recruitment 추가 | 성진우 | 
| 2026.06.01 | 1.7.0 | Deleting RecruitPost 삭제 | 성진우 | 
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

 인간은 사회적 동물이다’라는 아리스토텔레스의 말처럼 인간은 타인과 관계를 맺고 공동체를 이루며 살아가는 존재이다. 현대사회에서 사람들은 가족, 친구, 직장 등 다양한 관계 속에서 살아가며, 최근에는 바쁜 일상 속에서도 취미 기반의 소모임을 통해 스트레스를 해소하려는 경향이 증가하고 있다. 특히, 특히, 최근 주목받고 있는 ‘감자튀김 모임’과 같은 사례는 취미 기반 소모임이 증가하고 있는 흐름을 보여주는 대표적인 예로, 단순히 감자튀김을 먹으며 이야 나누다가 헤어지는 이 모임은 짧고 부담 없는 만남을 통해 2030 세대에게 큰 관심을 받고 있다.  
 
 이러한 흐름에 따라 취향 공유 플랫폼 또한 빠르게 성장하고 있다. 대표적으로 당근마켓은 기존 중고거래 중심 서비스에서 지역 기반 커뮤니티로 확장하며 ‘모임’ 기능을 도입하였고, 출시 1년 만에 이용자 수 1500만 명을 돌파하였다. 모임 개설 수와 가입자 수 또한 크게 증가하며 현대 사회에서 모임이 중요한 사회적 활동으로 자리잡고 있음을 보여준다.  
 
 그러나 대학 환경에서는 상황이 다소 다르다. 대학에서의 모임은 단순한 취미 활동을 넘어 조별과제, 공모전, 종합설계 프로젝트 등 평가와 직결되는 경우가 많다. 이러한 팀 프로젝트는 협업 능력, 의사소통 능력, 문제 해결 능력을 기를 수 있는 중요한 경험이지만, 동시에 높은 피로도를 유발하는 요소로 작용한다. 특히 학업, 아르바이트, 개인 일정 등으로 바쁜 대학생들에게는 팀원 모집과 일정 조율 자체가 큰 부담으로 작용한다. 
 
 실제로 많은 학생들이 팀 프로젝트의 중요성을 인식하면서도 팀 구성의 어려움으로 인해 참여를 꺼리는 경우가 많다. 또한 관련 정보를 쉽게 접하지 못하거나, 팀원을 구하기 위한 적절한 플랫폼이 부족하다는 문제도 존재한다. 기존의 익명 커뮤니티는 다양한 주제가 혼재되어 있어 팀원 모집에 적합하지 않으며, 익명성으로 인해 지원자의 정보(기술 스택, 경험 등)를 별도로 확인해야 하는 번거로움이 발생한다. 특히 컴퓨터공학 분야에서는 사용 언어, 개발 경험, 기술 스택 등 고려해야 할 요소가 많아 이러한 문제는 더욱 두드러진다.  
 
 이러한 문제를 해결하기 위해 대학생을 대상으로 한 팀원 매칭 및 팀 운영 지원 플랫폼 **‘Creation Time’** 를 개발하고자 한다.본 시스템의 목표는 **‘효율적인 팀원 모집’** 과 **‘원활한 팀 운영’** 이다. 사용자는 원하는 주제로 팀을 생성할 수 있으며, 팀 생성 시 자동으로 팀 리더 권한이 부여된다. 이후 팀 리더는 모집글을 작성하고, 지원자들의 정보를 체계적으로 확인한 뒤 간단한 조작을 통해 승인 또는 거절을 수행할 수 있다.팀이 구성된 이후에는 팀 페이지를 중심으로 다양한 협업 기능이 제공된다. 팀원 목록 확인, 일정 등록 및 공유, 투표를 통한 의사결정, 게시판을 통한 정보 공유 및 의사소통 기능을 통해 팀 운영을 효율적으로 지원한다. 또한 팀 리더는 팀원 관리 기능을 통해 팀 구성을 조정할 수 있으며, 투표 결과 및 지원자 현황을 파일 형태로 내보내어 관리 효율성을 높일 수 있다.  
 
  본 시스템은 단순한 모임 플랫폼을 넘어, 대학생들이 팀 프로젝트를 보다 효율적으로 수행할 수 있도록 지원하는 것을 목표로 한다.
  
---

# 2. System Context Diagram

<img width="1123" height="727" alt="image" src="https://github.com/user-attachments/assets/db9f7cdf-888c-4a7b-9759-e6e35c9a9fa8" />

## 기능 목록 

| 기능 | 설명 |
|------|------|
| Signing Up | 회원가입 |
| Logging In | 로그인 |
| Creating Team | 팀 만들기 |
| Creating Recruit Post | 팀원모집글(RecruitPost) 작성 |
| Viewing Recruit Post | 팀원모집글 조회 |
| Applying to Team | 팀 지원 |
| Reviewing Application | 팀 승인/거절 |
| Changing Role | 팀원 역할 변경 |
| Dismissing Team Member | 팀원 해고 |
| Creating Vote | 투표 생성 |
| Participating Vote | 투표 참여 |
| Viewing Vote Result | 투표 결과 확인 |
| Creating Schedule | 일정 등록 |
| Viewing Schedule | 일정 조회 |
| Writing Post | 팀 게시글 작성 |
| Viewing Post | 팀 게시글 확인 |
| Writing Comment | 팀 게시글에 댓글 작성 |
| Exporting Data | 엑셀로 데이터 내보내기 |
| Modifying Recruit Post | 팀원모집글 수정 |
| Modifying Post | 팀 게시글 수정 |
| Deleting Post | 팀 게시글 삭제 |
| Deleting Vote | 투표 삭제 |
| Deleting Schedule | 일정 삭제 |
| Deleting Comment | 팀 게시글의 댓글 삭제 |
| Deleting Team | 팀 해체 |
| Starting Recruitment |	팀원 모집 시작 |
| Closing Recruitment |	팀원 모집 중단 |


---


# 3. Use Case List

이 장은 프로젝트에서 사용될 use case list를 간략하게 설명하였다. Actor는 역할에 따라 가입을 안 한 사용자 Guest, 가입은 했지만 팀에 속하지 않은 RegisteredUser, 팀에 속한 TeamMember, 팀을 생성/관리하는 TeamLeader로 구분된다.


## 1) Signing Up

| Actor | Description |
|------|-------------|
| Guest | 사용자는 시스템을 이용하기 위해 회원가입을 수행한다. 사용자는 이름, 이메일 등 기본 정보와 필요에 따른 기술 스택에 관한 정보를 입력한다. 회원가입시에는 모든 사용자는 RegisteredUser로 지정된다. |

## 2) Logging In

| Actor | Description |
|------|-------------|
| Guest  | 사용자는 ID와 비밀번호를 통해 인증을 수행하고 시스템에 로그인하며, 패널티 점수에 따라 접근이 제한될 수 있다. TeamLeader는 추가적으로 팀 관리 기능을 사용할 수 있다. |

## 3) Creating Team

| Actor | Description |
|------|-------------|
| RegisteredUser | 사용자가 팀을 만든다. 팀의 이름, 설명, 모집 요건들을 입력하며, 팀 창설시 해당 사용자는 TeamLeader권한을 부여받는다. |

## 4) Creating Recruit Post

| Actor | Description |
|------|-------------|
| TeamLeader | 팀원 모집을 위한 RecruitPost을 작성한다. 팀의 목적, 요구조건, 활동계획 등의 정보가 포함되어야 한다. 해당 기능은 CreateTeam이후 TeamLeader여야만 가능하다. 작성된 글은 팀원 모집글 게시판에 등록된다. |

## 5) Viewing Recruit Post

| Actor | Description |
|------|-------------|
| Guest, RegisteredUser, TeamLeader | 팀원 모집글 게시판에서 RecruitPost을 조회하여 팀의 목적, 요구조건, 활동계획 등의 정보를 확인한다. |

## 6) Applying to Team

| Actor | Description |
|------|-------------|
| RegisteredUser | RecruitPost을 확인하고, 관심있는 팀에 지원한다. |

## 7) Reviewing Application

| Actor | Description |
|------|-------------|
| TeamLeader | 팀에 들어온 Application 목록을 확인하고 신청을 수락한다. 각 지원자에 대해 세부 정보를 확인할 수 있으며 승인 또는 거절을 통해 팀원을 선정할 수 있다. 승인된 사용자는 팀페이지에 접근 할 수 있다. |

## 8) Changing Role

| Actor | Description |
|------|-------------|
| TeamLeader | 팀 리더는 팀에 소속된 팀원들에게 특정 역할(예: 서버, UI 디자인, 부팀장, 서기 등)을 부여하거나 기존 역할을 수정할 수 있다. 수정된 역할은 시스템의 팀 정보에 반영된다. |

## 9) Dismissing Team Member

| Actor | Description |
|------|-------------|
| TeamLeader | 팀 리더는 특정 팀원을 팀에서 제외시킬 수 있다. 팀원 제외 시 해고 사유를 선택해야 하며, 불건전 사유에 해당할 경우 시스템은 해당 사용자에게 패널티 점수(Penalty Score)를 부과하여 상태에 영향을 줄 수 있다. |

## 10) Creating Vote

| Actor | Description |
|------|-------------|
| TeamLeader | 원활한 의사결정을 위해 다양한 투표를 만들 수 있다. 투표에 누가 참여했는지 확인이 가능하다. |

## 11) Participating Vote

| Actor | Description |
|------|-------------|
| TeamMember, TeamLeader | 팀 리더가 올린 투표에 참여 가능하다. 투표는 설정된 시간내에 수정가능하며, 투표시 항목별 투표현황을 확인 할 수 있다 |

## 12) Viewing Vote Result

| Actor | Description |
|------|-------------|
| TeamMember, TeamLeader | 이전에 진행된 투표 결과를 확인할 수 있다. 확인은 가능하지만, 수정은 불가능하다. |

## 13) Creating Schedule

| Actor | Description |
|------|-------------|
| TeamLeader | 팀페이지에 존재하는 캘린더에 일정을 등록한다. 캘린더에 라인 형태로 표시되며, 하단부에 정리된 형태로 표시한다. |

## 14) Viewing Schedule

| Actor | Description |
|------|-------------|
| TeamUser | 팀 페이지의 캘린더 또는 일정 목록에서 특정 일정을 선택하여 상세 정보를 조회한다. 선택된 일정은 강조 표시되며, 하단 영역에 일정의 세부 내용이 표시된다. |

## 15) Writing Post

| Actor | Description |
|------|-------------|
| TeamMember, TeamLeader | 팀페이지에서 글을 작성할 수 있다. |

## 16) Viewing Post

| Actor | Description |
|------|-------------|
| RegisteredUser, TeamMember, TeamLeader | 다른 사용자가 작성한 팀게시글을 확인하여 팀 활동과 관련된 정보를 조회한다. |

## 17) Writing Comment

| Actor | Description |
|------|-------------|
| TeamMember, TeamLeader | 팀 게시글 하단에 댓글을 작성하여 팀원 간 의견을 공유하고 의사소통을 수행한다. |

## 18) Exporting Data

| Actor | Description |
|------|-------------|
| TeamLeader | 팀 신청 명단, 투표 결과등을 csv 파일 형식으로 다운로드 받을 수 있다. |

## 19) Modifying Recruit Post

| Actor | Description |
|------|-------------|
| TeamLeader | TeamLeader가 작성한 팀원 모집글을 수정한다. |

## 20) Modifying Post

| Actor | Description |
|------|-------------|
| TeamMember, TeamLeader | 팀 게시글을 수정한다. |

## 21) Deleting Post

| Actor | Description |
|------|-------------|
| TeamMember, TeamLeader | 팀 게시글을 삭제한다. |

## 22) Deleting Vote

| Actor | Description |
|------|-------------|
| TeamLeader | TeamLeader가 투표를 삭제한다. |

## 23) Deleting Schedule

| Actor | Description |
|------|-------------|
| TeamLeader | TeamLeader가 등록된 일정을 삭제한다. |

## 24) Deleting Comment 

| Actor | Description |
|------|-------------|
| TeamMember, TeamLeader | 팀 게시글에 작성된 댓글을 삭제한다. |

## 25) Deleting Team

| Actor | Description |
|------|-------------|
| TeamLeader | TeamLeader가 팀을 해체한다. |

## 26) Starting Recruitment

| Actor | Description |
|------|-------------|
| TeamLeader | RecruitPost를 게시하며 모집을 시작한다. |

### 27) Closing Recruitment
| Actor | Description |
|------|-------------|
| TeamLeader | TeamLeader가 모집을 중단한다. |


---


# 4. Concept of Operation

## 1) Signing Up

| 항목 | 내용 |
|------|------|
| Purpose | Guest가 시스템을 이용하기 위한 계정을 생성할 수 있도록 한다. |
| Approach | Guest는 이름, ID, 비밀번호, 이메일 등 기본 정보와 희망하는 팀의 주제, 스택등을 입력하여 회원가입을 요청하고, 시스템은 이를 데이터베이스에 저장한다. |
| Dynamics | Guest가 회원가입 화면에서 정보를 입력하고 제출할 경우 |
| Goals | Guest 계정을 생성하여 시스템을 사용할 수 있다. 서버는Guest의 정보를 받아 저장하여 다른 Operation에 활용될 정보를 수집한다. |

## 2) Loging in

| 항목 | 내용 |
|------|------|
| Purpose | 등록된 RegisteredUser, TeamMember, TeamLeader의 인증을 통해 시스템에 접근할 수 있도록 한다. |
| Approach | Guest가 ID와 비밀번호를 입력하면 시스템은 입력된 정보를 기반으로 사용자 인증을 수행한다. 인증에 실패할 경우 오류 메시지를 출력하며, TeamMember, TeamLeader 혹은 RegisteredUser에게 부여된 패널티 점수에 따라 시스템 접근이 제한될 수 있다. |
| Dynamics |Guest가 로그인 요청을 보낼 누를 경우 |
| Goals | ID와 비밀번호를 통해 RegisteredUser, TeamMember, TeamLeader가 자신을 인증하여 자신에게 주어진 권한을 획득하며 상태에 따라 접근이 제한될 수 있다. |

## 3) Creating Team

| 항목 | 내용 |
|------|------|
| Purpose | RegisteredUser가 새로운 팀을 생성할 수 있도록 한다. |
| Approach | RegisteredUser는 팀 정보를 입력하고 팀 생성 버튼을 누르면 시스템은 이를 데이터베이스에 저장하고 요청한 RegisteredUser에게 TeamLeader 권한을 부여한다. |
| Dynamics | RegisteredUser가 팀 생성 요청을 수행할 경우 |
| Goals | RegisteredUser가 시스템으로부터 권한을 부여받아 TeamLeader로 승격된다. 최소 활동 단위인 Team을 형성한다. |

## 4) Creating Recruit Post

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 RecruitPost을 작성할 수 있도록 한다. |
| Approach | TeamLeader는 모집 관련 정보를 입력하여 게시글을 작성한다. |
| Dynamics | TeamLeader가 팀원을 모으기 시작할 때, RecruitPost을 작성할 때 |
| Goals | RecruitPost을 작성하여 팀원 모집글 게시판에 글이 올라오고, 다른 RegisteredUser가 팀에 가입할 수 있게 된다. |

## 5) Viewing Recruit Post

| 항목 | 내용 |
|------|------|
| Purpose | Guest, RegisteredUser, TeamLeader가 팀원 RecruitPost을 조회하여 팀 정보를 확인할 수 있도록 한다. |
| Approach | Guest, RegisteredUser, TeamLeader는 팀원 모집글 게시판에서 특정 게시글을 선택하여 상세 내용을 확인한다. |
| Dynamics | Guest, RegisteredUser, TeamLeader가 RecruitPost을 선택할 경우 |
| Goals | Guest, RegisteredUser가 팀 정보를 확인하고 지원 여부를 판단할 수 있고 TeamLeader는 정상적으로 작성되었는지 확인할 수 있다.  |

## 6) Applying Team

| 항목 | 내용 |
|------|------|
| Purpose | RegisteredUser가 관심 있는 팀에 지원할 수 있도록 한다. |
| Approach | RegisteredUser는 RecruitPost을 확인하고 모집글 하단부에 있는 버튼을 눌러 해당 팀에 지원할 수 있다. |
| Dynamics | RegisteredUser가 팀 지원 버튼을 누를 경우 |
| Goals | RegisteredUser가 신청 팀의 지원자 목록에 추가된다. |

## 7) Reviewing Application

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 팀 지원자를 승인/거절 할 수 있도록 한다. |
| Approach | TeamLeader는 Application 목록과 각 지원자의 기본 정보 및 희망 주제를 확인할 수 있다. TeamLeader가 승인 또는 거절을 선택하며 승인을 누를 경우 팀 정보에 팀원을 추가한다. |
| Dynamics | TeamLeader가 Application 목록을 확인할 경우 |
| Goals | TeamLeader가 승인/거절을 통해 팀원을 선정하고, 승인된 RegisteredUser가 팀 정보에 추가된다. |

## 8) Changing Role
| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 TeamMemver의 역할을 변경하거나 새롭게 부여할 수 있도록 한다. |
| Approach | TeamLeaderrk 특정 팀원의 역할을 입력하고 저장하며, 시스템은 팀 정보에 해당 변경을 반영한다. |
| Dynamics | TeamLeader가 팀원 역할 변경 작업을 수행할 경우 |
| Goals | 팀원들에게 역할을 지정하여 서로의 역할을 명확히 확인할 수 있도록 한다. |

## 9) Dismissing Team Member
| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 팀 구성을 관리하기 위해 특정 팀원을 팀에서 제외시킬 수 있도록 한다. |
| Approach | TeamLeader는 팀 관리 페이지에서 팀원을 선택하여 해고(제외)를 요청하고 사유를 선택한다. 시스템은 해당 팀원을 팀에서 제거하며, 사유에 따라 Penalty Score를 부과할 수 있다. |
| Dynamics | TeamLeader가 팀원 제외(해고) 작업을 수행할 경우 |
| Goals | 부적절한 활동을 하는 팀원을 관리하고 팀 구성을 최신화하며, 필요 시 제재를 가할 수 있다. |

## 10) Creating Vote

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 의사결정을 위한 투표를 생성할 수 있도록 한다. |
| Approach | TeamLeader는 투표 정보를 입력하여 투표를 생성한다. |
| Dynamics | TeamLeader가 투표를 생성할 경우 |
| Goals | TeamLeader가 안건에 대하여 투표를 생성할 수 있다. |

## 11) Participating Vote

| 항목 | 내용 |
|------|------|
| Purpose | TeamMember, TeamLeader가 투표에 참여할 수 있도록 한다. |
| Approach | TeamMember, TeamLeader는 투표의 선택 항목 중 하나를 선택하여 투표에 참여할 수 있으며, 참여 결과는 즉시 반영된다. |
| Dynamics | TeamMember, TeamLeader가 투표에 참여할 경우 |
| Goals | TeamMember, TeamLeader의 선택이 반영되어 투표 결과가 갱신된다. |

## 12) Viewing Vote Result

| 항목 | 내용 |
|------|------|
| Purpose | TeamMember, TeamLeader가 투표 결과를 확인할 수 있도록 한다. |
| Approach | TeamMember, TeamLeader는 기존에 생성된 투표를 선택하여 항목별 결과를 확인한다. |
| Dynamics | TeamMember, TeamLeader가 투표 결과를 조회할 경우 |
| Goals | TeamMember, TeamLeader가 항목별 투표 결과를 확인할 수 있다. |

## 13) Creating Schedule

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 팀 일정을 등록할 수 있도록 한다. |
| Approach | TeamLeader는 팀 페이지에 존재하는 캘린더에 일정을 눌러 추가할 수 있다. 추가 시 캘린더에 선 형태로 표시되며, 캘린더 하단부에서 요약된 일정을 확인할 수 있다. |
| Dynamics | TeamLeader가 일정을 등록할 경우 |
| Goals | TeamMember들이 일정을 한눈에 확인할 수 있다. |

## 14) Viewing Schedule

| 항목 | 내용 |
|------|------|
| Purpose | TeamUser가 팀의 일정 정보를 직관적으로 확인하고, 특정 일정의 상세 내용을 파악할 수 있도록 한다. |
| Approach | TeamUser는 팀 페이지의 캘린더 또는 일정 목록에서 특정 날짜나 일정을 선택한다. 시스템은 해당 일정의 상세 정보를 하단 영역에 표시하며, 선택된 일정은 강조 상태로 표시한다. |
| Dynamics | TeamUser가 일정이 표시된 날짜 또는 일정 항목을 클릭할 경우 |
| Goals | TeamUser가 특정 일정의 세부 내용을 쉽게 확인할 수 있다. |

## 15) Writing Post

| 항목 | 내용 |
|------|------|
| Purpose | TeamMember, TeamLeader가 팀 페이지내에 게시글을 작성하여 팀원 간 정보 공유 및 공지를 남길 수 있도록 한다. |
| Approach | TeamMember, TeamLeader는 팀 게시글을 작성하고 시스템은 이를 저장하여 다른 팀원이 확인할 수 있도록 한다. |
| Dynamics | TeamMember, TeamLeader가 팀 페이진에서 게시글을 작성할 경우 |
| Goals | 게시글을 통하여 진행에 필요한 정보를 공유하거나 TeamLeader가 공지를 남길 수 있다. |

## 16) Viewing Post

| 항목 | 내용 |
|------|------|
| Purpose  | RegisteredUser, TeamMember, TeamLeader가 게시글을 조회할 수 있도록 한다. |
| Approach | 사용자는 게시글 목록에서 특정 게시글을 선택하여 내용을 확인할 수 있다. |
| Dynamics | 사용자가 게시글을 선택할 경우 |
| Goals    | 사용자가 게시글을 통해 필요한 정보를 확인할 수 있다. |

## 17) Writing Comment

| 항목 | 내용 |
|------|------|
| Purpose  | RegisteredUser TeamMember, TeamLeader가 게시글에 댓글을 작성하여 의견을 공유할 수 있도록 한다. |
| Approach | RegisteredUser,TeamMember, TeamLeader는 게시글 하단의 입력창에 댓글을 작성하고 등록 버튼을 통해 의견을 남긴다. |
| Dynamics | RegisteredUser, TeamMember, TeamLeader가 게시글에 댓글을 작성후 등록 버튼을 누를시 |
| Goals | 게시글을 기반으로 사용자 간 의사소통이 이루어진다. |

## 18) Exporting Data

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 팀 관리 데이터를 외부에서 활용할 수 있도록 한다. |
| Approach | TeamLeader는 팀 신청 명단, 팀원 명단, 투표 결과를 CSV 파일 형식으로 생성하여 다운로드를 제공받을 수 있다. |
| Dynamics | TeamLeader가 데이터 다운로드 버튼을 누를 경우 |
| Goals | Team 정보가 필요할 때 내려받아 추가적인 작업을 진행할 수 있다. 해당 기능은 다른 정보도 내낼 수 있는 기반이 된다. |

## 19) Modifying Recruit Post

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 팀원 모집글을 수정할 수 있도록 한다. |
| Approach | TeamLeader는 기존 모집글을 수정한 뒤 변경 사항을 저장한다. |
| Dynamics | TeamLeader가 모집글 수정 기능을 선택할 경우 |
| Goals | 모집글의 내용이 최신 정보로 갱신된다. |

## 20) Modifying Post

| 항목 | 내용 |
|------|------|
| Purpose | TeamMember, TeamLeader가 팀 게시글을 수정할 수 있도록 한다. |
| Approach | TeamMember, TeamLeader는 기존 게시글을 수정한 뒤 저장한다. |
| Dynamics | TeamMember, TeamLeader가 게시글 수정 기능을 선택할 경우 |
| Goals | 팀 게시글의 내용이 최신 상태로 유지된다. |

## 21) Deleting Post

| 항목 | 내용 |
|------|------|
| Purpose | TeamMember, TeamLeader가 팀 게시글을 삭제할 수 있도록 한다. |
| Approach | TeamMember, TeamLeader는 삭제할 게시글을 선택하고 삭제를 요청하여 게시글을 제거한다. |
| Dynamics | TeamMember, TeamLeader가 게시글 삭제 기능을 선택할 경우 |
| Goals | 더 이상 필요하지 않은 팀 게시글이 게시판에서 제거된다. |

## 22) Deleting Vote

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 투표를 삭제할 수 있도록 한다. |
| Approach | TeamLeader는 삭제할 투표를 선택하고 삭제를 요청하여 투표를 제거한다. |
| Dynamics | TeamLeader가 투표 삭제 기능을 선택할 경우 |
| Goals | 더 이상 사용하지 않는 투표가 목록에서 제거된다. |

## 23) Deleting Schedule

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 일정을 삭제할 수 있도록 한다. |
| Approach | TeamLeader는 삭제할 일정을 선택하고 삭제를 요청하여 일정을 제거한다. |
| Dynamics | TeamLeader가 일정 삭제 기능을 선택할 경우 |
| Goals | 더 이상 필요하지 않은 일정이 캘린더와 일정 목록에서 제거된다. |

## 24) Deleting Comment

| 항목 | 내용 |
|------|------|
| Purpose | TeamMember, TeamLeader가 게시글에 작성된 댓글을 삭제할 수 있도록 한다. |
| Approach | TeamMember, TeamLeader는 게시글에 표시된 댓글 중 삭제할 댓글을 선택하고 삭제를 요청한다. |
| Dynamics | TeamMember, TeamLeader가 댓글 삭제 기능을 선택할 경우 |
| Goals | 불필요하거나 부적절한 댓글이 제거되어 게시글의 내용이 정리된다. |

## 25) Deleting Team

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 팀을 해체할 수 있도록 한다. |
| Approach | TeamLeader는 팀 해체를 요청하고 확인 절차를 거쳐 팀과 관련 데이터를 삭제한다. |
| Dynamics | TeamLeader가 팀 해체 기능을 선택할 경우 |
| Goals | 더 이상 사용하지 않는 팀이 시스템에서 제거된다. |

### 26) Starting Recruitment

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 RecruitPost을 게시판에 노출시키고 팀원 모집을 시작할 수 있도록 한다. |
| Approach | TeamLeader가 RecruitPost를 모집 중으로 전환하고 RecruitPost게시판에 노출한다. |
| Dynamics | TeamLeader가 모집 시작 기능을 선택할 경우|
| Goals | 팀원 모집을 공식적으로 시작하고, 다른 사용자가 모집글을 확인할 수 있게 한다. |

### 27) Closing Recruitment

| 항목 | 내용 |
|------|------|
| Purpose | TeamLeader가 모집을 중단하고 더 이상 게시판에 노출되지 않도록 한다. |
| Approach | TeamLeader가 모집을 중단하고 RecruitPost를 종료 상태로 전환, 모집 게시판에서 보이지 않도록 한다. |
| Dynamics | Team이 모두 형성되었거나 TeamLeader가 추가모집이 필요 없다고 판단한 경우 |
| Goals | 모집을 멈추고, 다시 시작할 수 있는 상태를 유지한다. |


---


# 5. Problem Statement

## Overviwe
Creation Time은 웹 기반의 팀원 매칭 및 일정 관리 프로그램이다. 팀리더가 팀 형성 후, RecruitPost을 쓰면 사용자가 신청하여 팀을 형성한다. 팀원 모집 이후에는 시간 결정등 팀 프로젝트 진행에서 일정 부드러운 일정조율을 위한 시간투표, 일정등록, 글작성등의 기능을 지원한다.

### Problem #1 – 직관적인 인터페이스
  본 시스템은 팀 페이지를 중심으로 다양한 기능과 정보가 동시에 제공되기 때문에 사용자에게 많은 정보가 한 번에 노출될 수 있다. 이로 인해 사용자가 원하는 정보를 찾거나 기능에 접근하는 데 어려움이 발생할 수 있으므로, 직관적인 정보 구조와 사용자 인터페이스 설계가 필요하다.

### Problem #2 – 다양한 디바이스 환경
  사용자는 모바일 기기와 데스크톱 환경 등 다양한 디바이스를 통해 시스템에 접근할 수 있다. 특히 간단한 조회는 모바일에서, 팀 운영과 같은 복잡한 작업은 데스크톱 환경에서 이루어질 가능성이 높다. 따라서 디바이스 특성에 맞는 사용자 인터페이스를 제공할 수 있는 설계가 필요하다.

### Problem #3 – 모임 구분
 공모전, 스터디는 다양한 분야가 존재한다. 전공, 관심사에 따라 만들어질 팀의 종류는 매우 다양하다. 해당 항목들을 효과적으로 정리할 수 있는 분류가 필요하다. 
 
### Problem #5 – 데이터 무결성과 일관성
본 시스템은 사용자, 팀, 투표 등 다양한 데이터를 저장하며, 이들 간의 관계가 복잡하게 연결되어 있다. 특히 팀 지원 및 승인 과정에서 동시에 여러 요청이 발생할 경우 데이터의 일관성이 깨질 수 있으며, 모집 상태, 지원 상태, 투표 상태 등 다양한 상태 변화 또한 체계적으로 관리되어야 한다. 따라서 데이터의 무결성과 일관성을 유지할 수 있는 저장 구조 설계가 필요하다.

### Problem #5 – 권한 및 역할 관리
팀 프로젝트에서는 팀 리더와 일반 팀원 간의 역할이 구분된다. 팀원 모집 승인, 일정 생성, 데이터 관리 등 특정 기능은 제한된 사용자만 수행해야 한다. 따라서 사용자 권한을 구분하고 이에 따라 기능 접근을 제어하는 설계가 필요하다.

### Problem #6 – 동시 접속 처리
  본 시스템은 팀 프로젝트를 위한 플랫폼으로, 다수의 사용자가 동시에 접속할 가능성이 높다. 따라서 여러 사용자의 요청을 안정적으로 처리할 수 있도록 동시 접근에 대한 고려가 필요하다.

  
---


# 6. Glossary

| 용어 | 설명 |
|------|------|
| Team | 하나의 주제를 가지고 활동하는 최소 활동 단위. 하나의 주제로 활동하는 최소 단위. 한명의 TeamLeader와 다수 TeamMember로 구성됨. |
| RecruitPost | TeamLeader가 RegisteredUser를 모집하기 위해 작성하는 게시물. |
| Application | 사용자가 특정 팀에 참여 의사를 밝힌 상태 또는 그 신청 내역 |
| Penalty Score | 사용자의 활동 상태를 반영하기 위한 값으로, 팀 활동 중 부적절한 행동 발생 시 증가할 수 있다. |


---


# 7. References

- https://topclass.chosun.com/news/articleView.html?idxno=35975  
- https://v.daum.net/v/0XJXDMB3lx?f=p  
- https://news.gknu.ac.kr/news/articleView.html?idxno=1802  
- https://www.asiatime.co.kr/article/20251105500311  
