📌 이 저장소는 프론트엔드 개발자 포트폴리오용으로 정리된 별도 README입니다.

<h1 align="center">안녕하세요 👋 김민석입니다</h1>
<h3 align="center">JavaScript 기반 기능 구현과 React 개발에 집중하고 있는 프론트엔드 개발자 김민석입니다.</h3>

👋 Welcome to My GitHub Portfolio!

안녕하세요! 저는 프론트엔드 개발자로서 **React, JavaScript, Firebase** 등 실무 중심 기술을 활용하여  
**사용자 친화적이며 기능 중심의 웹 애플리케이션**을 구현해왔습니다.  

단순한 퍼블리싱을 넘어, 데이터 저장, 인터랙션, API 연동 등 다양한 기능을 개발하며  
사용자 경험(UX)을 향상시키는 데 집중하고 있습니다.  

---

## 🔥 주요 프로젝트

### **1️⃣ 팀 프로젝트 리액트 가계부 웹앱**
- 🔗 [Demo 바로가기](http://popola1.dothome.co.kr/)
- 💻 [GitHub 소스 코드](https://github.com/kimminseock/Team-Project-Portfolio.git)
- 📄 [기능/역할 상세 PDF](https://github.com/kimminseock/ReactTeamProject_pdf.git)

**React와 Firebase를 활용한 수입/지출 관리 웹앱입니다.**  
실시간 데이터 동기화, CRUD, 차트 시각화, Excel 다운로드 등 다양한 기능을 구현했습니다.

- 수입/지출 등록, 수정, 삭제, 검색 기능
- 월별 통계 및 Recharts 기반 시각화
- Firebase Realtime Database를 활용한 실시간 데이터 저장
- Excel 다운로드 기능

- 🌱 **리액트 가계부 나의 기여도**
1. 화면 구성 및 기능 개발 (React):

   - React를 이용해 웹페이지 화면을 만들고, 데이터를 쉽게 입력할 수 있도록 구현

   - useState, useEffect를 사용해 화면이 자동으로 바뀌도록 설정

2. 데이터 저장 및 관리 (Firebase):

   - Firebase를 이용해 사용자의 수입/지출 기록을 저장하고 불러오는 기능 개발

3. 데이터 시각화 및 검색 기능:

   - Recharts 라이브러리를 이용해 월별 수입/지출을 그래프로 표시

   - 원하는 내역을 쉽게 찾을 수 있도록 검색 및 필터 기능 구현

4. ChatGPT API 연동:

   -  사용자의 소비 습관을 분석하고 간단한 조언을 제공하는 기능 개발

🧩 문제 해결 사례
- 🔸 **문제:** Firebase에서 데이터를 가져올 때 화면 반영 지연 발생  
  🔧 **해결:** 데이터를 받아온 후 화면에 바로 반영되지 않는 문제가 있어,  
  `useEffect`와 `onValue`를 함께 사용하여 **데이터가 변경되자마자 바로 화면이 업데이트되도록** 수정했습니다.

- 🔸 **문제:** 거래 내역 전체 불러오기 후 필터링하니 검색 속도 느림  
  🔧 **해결:** 처음엔 모든 데이터를 불러와서 필터링했지만,  
  **필요한 데이터만 쿼리로 가져오도록 `orderByChild`와 `equalTo`를 사용해** 검색 속도를 개선했습니다.

🛠 사용 기술:  
`React`, `Firebase`, `Recharts`, `XLSX`, `date-fns`, `ChatGPT API`, `HTML`, `CSS`, `JavaScript`

---

### **2️⃣ TodoList 웹앱 (Vanilla JS)**
- 🔗 [Demo 바로가기](http://popola1.dothome.co.kr/to_do_list/index.html)
- 💻 [GitHub 소스 코드](https://github.com/kimminseock/Todolist)

HTML/CSS와 순수 JavaScript로 제작한 CRUD 기능 완비형 투두리스트입니다.  
로컬스토리지, 다크모드, 반응형 디자인 등 실생활 사용성을 고려해 구현했습니다.

- 할 일 추가 / 목록 불러오기  
- 선택 삭제 / 마지막 항목 삭제 / 전체 삭제  
- 로컬스토리지로 데이터 유지  
- 다크모드 전환 (토글 스위치)  
- 모바일 최적화 반응형 UI  

🛠 사용 기술:  
`HTML5`, `CSS3`, `JavaScript (ES6+)`, `Web Storage API`

🧩 문제 해결 사례
- 🔸 **문제:** 다크모드 전환 시 일부 스타일이 초기화되는 현상 발생  
  🔧 **해결:** 다크모드 상태가 유지되지 않아서,  
  `document.documentElement` 기준으로 현재 모드를 저장하고,  
  **페이지 로딩 시에도 이전 모드가 적용되도록** 로직을 보완했습니다.

- 🔸 **문제:** localStorage에서 데이터 중복 출력  
  🔧 **해결:** 새로고침 후 할 일이 중복 출력되는 문제가 있어,  
  데이터를 다시 그리기 전에 `.innerHTML = ''`으로 **리스트를 먼저 초기화**한 뒤 다시 출력하도록 수정했습니다.

---

### **3️⃣ 제빵 만드는 방법 소개 사이트**
- 🔗 [Demo 바로가기](http://popola1.dothome.co.kr/bread/bakery.html)
- 💻 [GitHub 소스 코드](https://github.com/kimminseock/Personal-Portfolio.git)

**AI 이미지와 인터랙션 중심의 정보 제공형 웹사이트**입니다.  
CSS 애니메이션과 Web Animation API, IntersectionObserver 등을 활용하여 UX를 강화했습니다.

- 슬라이드 기능, AI 이미지 소개  
- 메인/서브 페이지로 구성된 구조  
- 반응형 설계, IntersectionObserver 활용  

🛠 사용 기술:  
`HTML5`, `CSS3`, `JavaScript`, `Web Animation API`, `IntersectionObserver`

📌 애니메이션 설계 전략:

- 메인 페이지는 텍스트 등장 및 슬라이드 전환 등 인터랙션을 `@keyframes` 기반의 CSS 애니메이션으로 구현하고,  
  JavaScript는 `.next`, `.prev` 클래스를 토글하는 트리거 역할만 수행합니다.  

- 반면, 서브 페이지는 `Web Animation API`를 활용하여  
  이미지의 **흑백 → 컬러 전환**, **IntersectionObserver**를 통한 요소 등장 애니메이션 등을 구성했으며,  
  **스크롤 기반 인터랙션 중심으로 섬세한 효과 구현**에 집중했습니다.

🧩 문제 해결 사례
- 🔸 **문제:** 모바일 메뉴 버튼 작동 불안정  
  🔧 **해결:** `toggle()` 방식으로만 열고 닫다 보니 간헐적으로 버튼이 먹히지 않았습니다.  
  그래서 `classList.contains()`로 **현재 열려 있는지 먼저 확인한 뒤**,  
  상태에 따라 열거나 닫는 동작을 구분해서 **더 안정적으로 작동하도록** 변경했습니다.

---

### **4️⃣ e-book 창작 사이트**
- 🔗 [Demo 바로가기](http://popola1.dothome.co.kr/e_book/index.html)
- 💻 [GitHub 소스 코드](https://github.com/kimminseock/e-book)

**웹 인터랙션과 콘텐츠 필터링이 강화된 전자책 창작 플랫폼**입니다.  
jQuery, Swiper.js, AOS, GSAP 등 다양한 라이브러리와 커스텀 코드를 혼합하여 풍부한 사용자 경험을 제공했습니다.

📌 주요 기능:
- 커스텀 메인 슬라이드: jQuery 기반 `.animate()` 슬라이더
- Swiper.js Coverflow / 카드 슬라이드 효과
- 카테고리 클릭 → AOS 애니메이션 재실행 구조
- GSAP ScrollTrigger 기반 섹션 배경 전환
- 책 소개 영역 타이핑 애니메이션
- 모바일 기준 반응형 레이아웃 구성

🛠 사용 기술:  
`HTML5`, `CSS3`, `JavaScript`, `jQuery`, `Swiper.js`, `GSAP`, `ScrollTrigger`, `AOS`

🧩 문제 해결 사례
- 🔸 **문제:** GSAP ScrollTrigger와 AOS 충돌로 애니메이션 중복 실행  
  🔧 **해결:** AOS는 `once: true` 옵션으로 한 번만 실행되게 하고,  
  GSAP은 `refresh()`를 사용해서 **초기화 시점을 명확히 잡아 충돌을 방지했습니다.**

- 🔸 **문제:** 모바일에서 Swiper Coverflow가 깨짐  
  🔧 **해결:** 작은 화면에서는 슬라이드가 잘리지 않거나 깨졌는데,  
  `breakpoints` 옵션을 설정하고 슬라이드 수를 줄여서 **모바일에서도 안정적인 슬라이드 형태를 유지하도록** 수정했습니다.

---

## 🧰 기술 스택

<table>
  <tr>
    <td align="center"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" width="40"><br>JavaScript</td>
    <td align="center"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" width="40"><br>React</td>
    <td align="center"><img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" width="40"><br>Firebase</td>
    <td align="center"><img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" width="40"><br>Figma</td>
    <td align="center"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" width="40"><br>HTML5</td>
    <td align="center"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" width="40"><br>CSS3</td>
    <td align="center"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/jquery/jquery-original.svg" width="40"><br>jQuery</td>
  </tr>
</table>

🔧 추가 기술:  
`Recharts`, `XLSX`, `date-fns`, `ChatGPT API`, `Swiper.js`, `GSAP`, `AOS`, `Web Animation API`

---

## 🌱 기타 경험 및 협업 도구

- Git / GitHub 기반 버전 관리 및 팀 프로젝트 경험  
- Figma를 통한 UI 설계 이해 및 CSS 구현  
- Firebase 실시간 데이터 처리 및 API 연동 경험  
- 반응형 웹 제작 시 모바일 퍼스트 전략 적용

---

📫 **이메일:** popola22@naver.com  
📱 **연락처:** 010-6656-7464
