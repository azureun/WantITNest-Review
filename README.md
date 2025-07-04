# 🪺 WantIT-Nest
> 흩어진 사람들과 정보를 하나로, 함께 성장하는 IT 커뮤니티 플랫폼

**배포 주소**: [https://wantitnest.co.kr](https://wantitnest.co.kr) <br>
- Tip : 재학생 이메일 주소인 @chosun.ac.kr로 로그인하면 프로필에 재학생 인증 배찌가 나타납니다.


## 🧭 개발 목적

WantIT-Nest는 조선대학교 IT융합대학 재학생들이 겪는 진로 탐색, 정보 접근, 교내 교류의 어려움을 실질적으로 해결하기 위해 개발된 커뮤니티 플랫폼입니다.

- 많은 재학생들이 진로 방향 설정에 막막함을 느끼고 있으나, 졸업생과의 연결 기회가 부족해 현실적인 조언을 듣기 어렵습니다.  
- 또한 학과 공지사항, 프로그램 안내 등 학교 정보가 여러 플랫폼에 분산되어 있어 필요한 정보를 한눈에 확인하기 힘든 구조입니다.  
- 팀 프로젝트 경험 및 커리어 모델 부족 문제로 진로 준비에 있어 어려움을 겪고 있습니다.

이러한 문제를 해결하기 위해 WantIT-Nest는 다음을 목표로 선정하였습니다:

1. **졸업생과의 네트워킹 기능**을 통해 진로 경험과 조언을 공유  
2. **관심 분야 기반의 교류 공간**으로 팀 프로젝트 및 정보 공유 활성화  
3. **학교 정보 통합 제공**으로 효율적인 정보 접근 환경 구축  
4. **실전 기반 커리어 설계 환경**을 통해 전공자의 성장 지원

WantIT-Nest는 IT융합대학 구성원이 함께 연결되고, 함께 성장하며, 함께 진로를 설계할 수 있도록 돕는 것을 목표로 합니다.

## 🔎 프로젝트 개요
- 기획 기간 : 2025.03.06~2025.03.22
- 개발 기간 : 2025.03.24~2025.06.23 (총 14주)
- 개발 인원 : 총 7인
    - 프론트엔드(3명), 백엔드(3명), AI/Data(1명)
- 담당 역할 : 프론트엔드 개발
    - React + TypeScript 기반 SPA(Single Page Application)

## ⚙️ 기술 스택 및 아키텍쳐
**기술 스택**<br>
- Frontend
    - React.js, TypeScript, TailwindCSS, Styled-Components
    - React Router, Redux Toolkit, React Markdown
    - Vite
- Backend
    - Java 17 (Eclipse Temurin), Spring Boot 3.4.3- REST API, Spring Security (JWT 기반 인증/인가)
    - MySQL 8.0.33 (JPA 기반 ORM)
- 실시간/AI 서비스
    - Node.js + Socket.IO (실시간 채팅)
    - Python FastAPI + OpenAI GPT-4o API (AI 챗봇)
    - BeautifulSoup + Selenium (공지 크롤러)
- DevOps & Infra
    - Docker / Docker Compose
    - AWS EC2 기반 2-Tier 구조 (Public + Private Subnet)
    - GitLab + Git Subtree (멀티 레포지터리 통합 관리, 학교 과제 제출용)

**시스템 아키텍쳐**<br>
<img src="./review-src/WantIT-Nest System Architecture.png" width="500" height="550" />

### 💾 원본 Repository (Github Organization)
- Front-end : [chosun-nest/Nest-FE](https://github.com/chosun-nest/Nest-FE)
- Back-end : [chosun-nest/Nest-BE](https://github.com/chosun-nest/Nest-BE)
- Crawl : [NEST-AI/tree/dev](https://github.com/chosun-nest/NEST-AI/tree/dev)
- Chat-bot : [Nest-CB/tree/dev](https://github.com/chosun-nest/Nest-CB/tree/dev)

## 🔭 주요 기능
> 담당 : **굵은 글씨**로 나타낸 부분
- 메인 페이지: 관심 태그 기반 콘텐츠 요약, 공지/모집글/인기글 통합 표시
- 프로필 페이지(본인/다른 사용자) : **프로필 카드**, 활동 히스토리, **팔로우 기반 소셜 연결**
- **회원정보 수정 페이지** : 프로필 정보(이미지, 기술스택, SNS 링크 설정 등), 비밀번호 변경, 회원 탈퇴
- 공지사항 게시판: 조선대 전공/사업단 공지를 자동 크롤링하여 통합 제공
- **관심분야 게시판**: 질문, 정보 공유, 경험담 나눔 등 마크다운 기반 커뮤니티
- 프로젝트 모집 게시판: 팀원 모집, 역할 기반 지원 시스템
- 실시간 채팅: 팔로우 기반 1:1 및 그룹 채팅 지원 (Socket.IO)
- AI 챗봇: OpenAI GPT-4o API를 활용한 FAQ + 자유 질문 응답 기능

## 💻 주요 화면/기능

> ### **로그인/회원가입**

- 로그인/비밀번호 재설정
<table>
  <tr>
    <td><img src="./review-src/로그인 페이지.png" width="400" height="200"/></td>
    <td><img src="./review-src/비밀번호 재설정 페이지.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>로그인 페이지</b></td>
    <td align="center"><b>비밀번호 재설정 페이지</b></td>
</table>

- 회원가입 페이지
<table>
  <tr>
    <td><img src="./review-src/회원가입 페이지1.png" width="400" height="200"/></td>
    <td><img src="./review-src/회원가입 페이지2.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>회원가입 페이지1</b></td>
    <td align="center"><b>회원가입 페이지2</b></td>
</table>

---

> ### **메인 페이지**
<table>
  <tr>
    <td><img src="./review-src/메인페이지(로그인 전).png" width="400" height="300"/></td>
    <td><img src="./review-src/메인페이지(로그인 후).png" width="400" height="350"/></td>
  </tr>
    <td align="center"><b>메인페이지(로그인 전)</b></td>
    <td align="center"><b>메인페이지(로그인 후)</b></td>
</table>

---

> ### **프로필**

- 프로필 페이지
<table>
  <tr>
    <td><img src="./review-src/본인 프로필 페이지.png" width="400" height="320"/></td>
    <td><img src="./review-src/다른 사용자 프로필 페이지.png" width="400" height="320"/></td>
  </tr>
    <td align="center"><b>본인 프로필 페이지</b></td>
    <td align="center"><b>다른 사용자 프로필 페이지</b></td>
</table>

- 팔로잉 기능
<table>
  <tr>
    <td><img src="./review-src/본인 팔로워 목록.png" width="400" height="200"/></td>
    <td><img src="./review-src/다른 사용자 팔로잉 목록.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>본인 팔로워 목록</b></td>
    <td align="center"><b>다른 사용자 팔로잉 목록</b></td>
</table>

---

> ### **회원 정보 수정 페이지**
<table>
  <tr>
    <td><img src="./review-src/회원정보 수정 페이지.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>회원정보 수정 페이지</b></td>
</table>

---

> ### **공지사항 게시판**

- 공지사항 게시판 페이지
<table>
  <tr>
    <td><img src="./review-src/공지사항 게시판 페이지.png" width="400" height="200"/></td>
    <td><img src="./review-src/IT융합대학 선택.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>공지사항 게시판 페이지</b></td>
    <td align="center"><b>IT융합대학 선택</b></td>
</table>

---

> ### **관심분야 정보 게시판**

- 관심분야 정보 게시판 페이지
<table>
  <tr>
    <td><img src="./review-src/관심분야 정보 게시판 페이지 1.png" width="400" height="200"/></td>
    <td><img src="./review-src/관심분야 정보 게시판 페이지 2.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>관심분야 정보 게시판 페이지 1</b></td>
    <td align="center"><b>관심분야 정보 게시판 페이지 2</b></td>
</table>

- 관심분야 정보 게시글 상세 페이지
<table>
  <tr>
    <td><img src="./review-src/관심분야 정보 게시글 상세 1.png" width="400" height="200"/></td>
    <td><img src="./review-src/관심분야 정보 게시글 상세 2.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>관심분야 정보 게시글 상세 1</b></td>
    <td align="center"><b>관심분야 정보 게시글 상세 2</b></td>
</table>

- 관심분야 정보/프로젝트 모집 글쓰기 페이지
<table>
  <tr>
    <td><img src="./review-src/관심분야 정보 글쓰기 페이지.png" width="400" height="200"/></td>
    <td><img src="./review-src/프로젝트 모집 글쓰기 페이지.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>관심분야 정보 글쓰기 페이지</b></td>
    <td align="center"><b>프로젝트 모집 글쓰기 페이지</b></td>
</table>

---

> ### **프로젝트 모집 게시판**

- 프로젝트 모집 게시판/상세 페이지
<table>
  <tr>
    <td><img src="./review-src/프로젝트 모집 게시판 페이지.png" width="400" height="200"/></td>
    <td><img src="./review-src/프로젝트 모집 게시판 상세.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>프로젝트 모집 게시판 페이지</b></td>
    <td align="center"><b>프로젝트 모집 상세 페이지</b></td>
</table>

---

> ### **채팅방**

<table>
  <tr>
    <td><img src="./review-src/채팅방 팔로잉 목록.png" width="400" height="200"/></td>
    <td><img src="./review-src/개인 채팅방.png" width="400" height="200"/></td>
  </tr>
    <td align="center"><b>채팅방 팔로잉 목록</b></td>
    <td align="center"><b>개인 채팅방</b></td>
</table>

---

> ### **챗봇**

<table>
  <tr>
    <td><img src="./review-src/FAQ 선택 답변.png" width="400" height="600"/></td>
    <td><img src="./review-src/GPT 4o API 활용한 답변.png" width="400" height="600"/></td>
  </tr>
    <td align="center"><b>FAQ 선택 답변</b></td>
    <td align="center"><b>GPT 4o API 활용한 답변</b></td>
</table>

---

## 👩🏻‍💻 담당 역할 및 기여 (기여도: 약 25%)

**🎨 Figma 프로토타입**

- UI 흐름 설계 및 주요 컴포넌트 디자인
- 페이지 전환 구조, 반응형 프로토타입 제작
- [Figma 링크 - only view](https://www.figma.com/proto/OOqaT6pOp85uw5IvfGjHy3/CSU-NEST?node-id=88-401&starting-point-node-id=88%3A401&t=2ZbxpxNXhCJWeDcg-1)

**🪪 프로필 관련**

- 본인/타인 프로필 페이지
    - 프로필 카드: 사용자 정보(이름, 학과, 재학생 여부), 기술 스택, SNS 링크, 프로필 수정 또는 팔로워/팔로잉 상태
- 회원 정보 수정 페이지
    - 프로필 이미지 업로드, 학과·기술 스택 검색, SNS 링크 설정
    - 비밀번호 변경, 회원 탈퇴 처리 (모달, API 연동 포함)

**🖼️ 관심분야 게시판 관련**

- 관심분야 정보 게시판 페이지
    - 검색, 정렬(좋아요순/최신순), 게시글 카드 렌더링
    - 글쓰기 버튼 위치별 분기 처리, 태그 검색(다중 선택 최대 10개)
- 관심분야 정보 글쓰기 페이지
    - 게시글 쓰기 유형 전환 드롭다운 (관심분야 정보 / 프로젝트 모집)
    - 태그 선택
- 관심분야 정보 게시글 상세 페이지
    - 게시글 - CRUD, 작성자 프로필 이동, 팔로잉, markdown 본문, 반응 처리(좋아요/싫어요/공유)
    - 댓글/대댓글 - CRUD, 대댓글 멘션(@), 댓글 트리 구성, 작성자 프로필 이동, 반응 처리(좋아요/싫어요)



