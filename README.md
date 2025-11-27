# Analytics Assistant - Portfolio

> 데이터 분석을 위한 웹 기반 셀프서비스 분석 플랫폼

## Live Demo

https://somoon0422.github.io/analytics-portfolio/

---

## 프로젝트 소개

**Analytics Assistant**는 SQL에 익숙하지 않은 비즈니스 사용자도 쉽게 데이터를 분석할 수 있도록 만든 웹 애플리케이션입니다.

### 개발 배경
- 데이터 분석 요청이 많아 분석가 업무 과부하
- SQL 작성이 어려운 비개발 직군의 데이터 접근성 문제
- 반복적인 쿼리 작성으로 인한 비효율

### 해결 방안
- 드래그 앤 드롭 기반 쿼리 빌더
- 자주 쓰는 쿼리 템플릿화 (원클릭 실행)
- AI 기반 자연어 → SQL 변환

---

## 주요 기능

### 1. 데이터 분석 도구 (기본 모드)
- 드래그 앤 드롭으로 컬럼 선택
- GROUP BY, 집계함수, WHERE 조건 자동 구성
- 실시간 SQL 미리보기 (구문 강조)

### 2. 원클릭 모드
- 카테고리별 쿼리 템플릿
- `{{변수명}}` 형식의 동적 변수 지원
- 실행 시 변수 입력 모달 자동 표시

### 3. AI 어시스턴트
- Claude AI 기반 자연어 쿼리
- 데이터 분석 결과 해석
- 컬럼 설명 및 가이드 제공

### 4. 컬럼 카탈로그
- Redshift 메타데이터 자동 동기화
- 컬럼별 설명, 예시값, 수식 정보
- 검색 및 필터 기능

### 5. 데이터 시각화
- Amazon QuickSight 연동
- 쿼리 결과 기반 차트 생성
- 대시보드 임베딩

---

## 기술 스택

| 구분 | 기술 |
|------|------|
| Backend | Node.js, Express.js |
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Database | Amazon Redshift |
| AI | Claude API (Anthropic) |
| 시각화 | Amazon QuickSight, Chart.js |
| 기타 | MCP SDK, xlsx, pptxgenjs |

---

## 아키텍처

```
┌─────────────────────────────────────────┐
│           Frontend (SPA)                │
│   HTML5 + CSS3 + Vanilla JavaScript     │
└─────────────────┬───────────────────────┘
                  │ REST API
┌─────────────────┴───────────────────────┐
│         Backend (Node.js/Express)       │
│  • Query Builder API                    │
│  • AI Chat API (Claude)                 │
│  • QuickSight Integration               │
└─────────────────┬───────────────────────┘
                  │
┌─────────────────┴───────────────────────┐
│          Amazon Redshift                │
│        (Data Warehouse)                 │
└─────────────────────────────────────────┘
```

---

## 성과

- 데이터 조회 시간 **70% 단축**
- 비개발 직군 데이터 접근성 **대폭 향상**
- 반복 쿼리 작성 업무 **자동화**

---

## 소스 코드

- 메인 저장소: [analytics-assistant](https://github.com/somoon0422/analytics-assistant)

---

## 개발자

**김소희**
- GitHub: [@somoon0422](https://github.com/somoon0422)

---

**Last Updated**: 2025-01-27
