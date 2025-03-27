# 🏗 BuilDone: 할 일 목록 웹 서비스 프로젝트
Team project to develop a complex to-do list web service.

## 📌 곽태근 역할 (ROLE)
- 랜딩 페이지 개발 (Landing Page)
- 모든 할 일 목록 페이지 개발 (All To-Do List Page)
- 내비게이션 바 개발 (Navigation/Tab-Side Bar)
- Todo 공통 컴포넌트 개발 (Todo Shared Component)
- Sentry 환경 구축 (Sentry: Error Tracking and Performance Monitoring)
- Jest 테스트 환경 구축 (Jest: Unit & Integration Testing)
- 노트 링크 임베드 기능 구현 (Link Embedded)

## 🔹 개발한 주요 Hooks
- useInView → 요소가 화면에 보일 때 이벤트 요청을 처리하는 훅
- useInfiniteScroll → 옵저버 기반 무한 스크롤 기능을 위한 훅

## 🚀 개발한 기능 상세 설명

### 1️⃣ 랜딩 페이지 개발 (Landing Page)
- tailwind.config에서 애니메이션 키워드 생성
- useInView 훅을 활용하여 요소가 화면에 보일 때 애니메이션 실행

### 2️⃣ 모든 할 일 목록 페이지 개발 (All To-Do List Page)
- TanStack Query와 useInfiniteScroll 훅을 활용하여 무한 스크롤 기능 구현
- 무한 스크롤 기능을 적용하는 과정에서 서버 상태 관리 및 비동기 데이터 처리에 대한 이해가 부족하여 어려움을 겪음
- 팀원과 협업하며 무한 스크롤 옵션 생성자를 활용하는 법을 익히고, 이후 코드를 올바르게 작성할 수 있었음

### 3️⃣ 내비게이션 바 개발 (Navigation/Tab-Side Bar)
- 내비게이션 바는 화면 크기에 따라 구조가 달라지는 UI/UX가 필요
- class-variance-authority 라이브러리를 활용, UI 스타일을 효율적으로 관리, 다양한 스타일 변형을 쉽게 적용
- 처음에는 복잡했지만, 유지보수성과 재사용성을 높이는 방법을 배울 수 있었음

### 4️⃣ Todo 공통 컴포넌트 개발 (Todo Shared Component)
- 다른 팀원들도 사용할 공통 컴포넌트로 개발
- 초반에 중요성을 인식하지 못해 늦게 개발했지만, 재사용 가능한 컴포넌트 설계의 중요성을 배움
- 프롭스(Props)와 조건문을 활용하여 여러 UI 구성에서 재사용 가능하도록 설계

### 5️⃣ Sentry / Jest 환경 구축
- 공식 문서 가이드를 참고하여 Sentry 및 Jest 환경 설정
- 빌드 과정에서 API 키 변경 및 환경 변수(.env) 업데이트 누락으로 인해 오류 발생
- 환경 변수 및 패키지 설정을 관리하는 중요성을 인식하고 개선

### 6️⃣ 노트 링크 임베드 기능 구현 (Link Embedded)
- 팀원의 작업 일정이 지연됨에 따라 추가 기능을 개발하게 됨
- 사용자가 웹사이트 링크를 입력하면 해당 링크를 사이트 내에서 직접 임베드
- 일부 웹사이트는 임베드를 허용하지 않기 때문에 예외 처리 필요
- fetch를 이용해 링크의 임베드 가능 여부를 확인하고, 불가능할 경우 대체 UI 제공

## 💡 프로젝트를 통해 배운 점
✅ 비동기 데이터 관리 및 상태 관리의 중요성  

✅ 공통 컴포넌트 설계 및 재사용성 극대화  

✅ 빌드 과정에서 환경 변수 및 패키지 설정을 철저히 관리하는 습관  

✅ 협업을 통해 팀원과의 소통이 얼마나 중요한지 경험
