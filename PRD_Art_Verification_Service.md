# Art Verification Service - Product Requirements Document

## 1. 제품 개요
### 목적
전세계 고객들이 소유한 미술품의 진위 여부를 AI 기술을 통해 검증할 수 있는 웹 기반 서비스

### 핵심 가치 제안
- 간편한 이미지 업로드만으로 미술품 진위 검증
- 전문가 수준의 AI 분석 결과 제공
- 글로벌 접근성과 다국어 지원

## 2. 핵심 기능

### 2.1 결제 시스템
- Stripe 결제 연동 (제공된 링크: https://buy.stripe.com/test_fZu4gB97J6wX1efakj1RC00)
- 검증 서비스 이용료: $9.99 per analysis
- 결제 완료 후 즉시 서비스 이용 가능

### 2.2 이미지 업로드 및 분석
- 지원 형식: JPG, PNG, WEBP (최대 10MB)
- AI 모델을 통한 가짜 미술품 검출
- Google Vision API 연동 (제공된 API 키 활용)
- 분석 결과: 진품 확률 % 및 상세 분석 리포트

### 2.3 결과 제공
- 실시간 분석 진행 상황 표시
- 상세 분석 리포트 (PDF 다운로드 가능)
- 이메일로 결과 발송 옵션

## 3. 기술 스택
- Frontend: HTML5, CSS3, JavaScript (Vanilla)
- Backend: Node.js/Express 또는 Python/Flask
- AI/ML: TensorFlow.js 또는 Python 기반 모델
- 결제: Stripe API
- 이미지 분석: Google Vision API
- 배포: Vercel/Netlify

## 4. 사용자 플로우
1. 랜딩 페이지 방문
2. 서비스 설명 확인
3. Stripe 결제 진행
4. 결제 완료 후 업로드 페이지 이동
5. 미술품 이미지 업로드
6. AI 분석 진행 (로딩 화면)
7. 결과 확인 및 리포트 다운로드

## 5. UI/UX 요구사항
- 반응형 디자인 (모바일 친화적)
- 직관적이고 깔끔한 인터페이스
- 다국어 지원 (영어, 한국어 우선)
- 빠른 로딩 시간과 부드러운 애니메이션

## 6. 보안 및 개인정보
- 업로드된 이미지는 분석 후 24시간 내 삭제
- HTTPS 통신 필수
- 개인정보 처리방침 명시