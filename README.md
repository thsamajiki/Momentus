# 🪄 Momentus
**개인 맞춤형 홈 화면 Chrome Extension 서비스**

> 반복적으로 사용하는 브라우저 새 탭 환경을 생산성 중심 인터페이스로 재해석한 서비스입니다.  
날씨, 시간, 명언, 할 일 등 개인화 요소를 기반으로 사용자의 하루를 정돈할 수 있도록 설계했습니다.

---

## 🚀 주요 기능

- 🕒 **실시간 시간 표시**
- 🌤 **OpenWeatherMap 기반 지역 날씨 표시**
- ✨ **랜덤 영감 문구 제공**
- 📝 **To-Do 리스트 관리**
- 🎨 **다크모드 및 사용자 테마 설정**
- 💾 **사용자 설정 및 데이터 자동 저장 (IndexedDB 기반)**

---

## 🧩 기술 스택

| 분야 | 사용 기술 |
|------|-----------|
| UI Framework | **React (TypeScript)** |
| 상태 및 데이터 | **React Query, IndexedDB + Dexie.js** |
| UI / 스타일 | **TailwindCSS, Emotion** |
| 플랫폼 | **Chrome Extension – Manifest V3** |
| API | **OpenWeatherMap API** |

---

## 🛠 주요 구현 포인트

### 1️⃣ Hooks 기반 성능 최적화
- `useState`, `useEffect`, `useMemo`를 활용해 **렌더링 비용 최소화**
- UI와 사용자 이벤트 간의 상태 연동 간결화

### 2️⃣ React Query 기반 API 캐싱 구조
- 비동기 API 호출 최소화
- Stale-While-Revalidate 전략 기반으로 UX 경험 개선

### 3️⃣ IndexedDB 기반 데이터 영속성
- `Dexie.js`를 이용해 `localStorage` 대비  
  **데이터 구조화·검색·확장성 개선**

### 4️⃣ TailwindCSS + Emotion 기반 UI 시스템 설계
- UI 레이어를 `컴포넌트 단위(Button, Widget, Card)`로 추상화
- 반응형 디자인 & 테마 커스터마이징 지원
- **유틸 기반 스타일링 + 세밀한 Emotion 스타일 병행 구조 확립**

### 5️⃣ Debugging & Developer Experience 개선
- Chrome DevTools + React Developer Tools 활용  
  → 렌더링 흐름, 상태 변화, 메모리 사용 추적

---

## 💡 개발 의도

> "매일 처음 여는 탭이라면, 단순한 페이지가 아니라 나에게 집중하는 공간이 될 수 있어야 한다고 생각했습니다.
Momentus는 단순한 기능을 모아둔 확장 프로그램이 아니라,
사용자의 하루를 준비할 수 있는 개인화된 디지털 데스크를 목표로 합니다."

---

## 📌 향후 개선사항

- 사용자 데이터 동기화 지원 (Google Sync Storage)
- 위젯 추가 및 자유 배치 기능
- 멀티 기기 설정 유지 기능

---

## 🧑‍💻 만든 사람

| Name	| Role |
|------|------|
| thsamajiki	| Android Developer 🚀 + React 경험 기반 확장 |
