# 🎨 ArtVerify - AI-Powered Art Authentication Service

**Global Art Verification Platform**

전세계 고객들이 소유한 미술품의 진위 여부를 AI 기술을 통해 검증할 수 있는 웹 기반 서비스입니다.

## 🌍 Features

- **AI Art Analysis**: 이미지 업로드 후 AI 기반 진위 검증
- **Global Payment**: Stripe를 통한 전 세계 결제 지원
- **Responsive Design**: 모바일, 태블릿, 데스크톱 최적화
- **Real-time Processing**: 실시간 분석 결과 제공
- **Subscription Management**: 구독 상태 확인 및 관리

## 🚀 Quick Start

### 로컬 실행
```bash
# Python HTTP 서버 실행
python -m http.server 8000

# 브라우저에서 접속
http://localhost:8000
```

### 글로벌 배포 (Vercel)

1. **Vercel CLI 설치**
```bash
npm install -g vercel
```

2. **배포 실행**
```bash
vercel --prod
```

3. **자동으로 생성되는 글로벌 URL로 접속**
   - 예: `https://artificial-ny.vercel.app`

## 💳 Payment Setup

### Stripe 연동 (실제 결제)
1. [Stripe](https://stripe.com) 계정 생성
2. 대시보드에서 Publishable Key 복사
3. `payment-stripe.js` 파일의 `STRIPE_PUBLIC_KEY` 교체

### 테스트 결제
- 카드번호: `4242 4242 4242 4242`
- 만료일: 미래 날짜
- CVC: 아무 3자리 숫자

## 📁 Project Structure

```
artificial-ny/
├── index.html              # 메인 페이지
├── payment-stripe.html     # Stripe 결제 페이지
├── payment-stripe.js       # Stripe 결제 로직
├── script.js              # 메인 기능 스크립트
├── styles.css             # 스타일시트
├── subscription-manager.js # 구독 관리
├── package.json           # 프로젝트 설정
├── vercel.json           # Vercel 배포 설정
└── README.md             # 프로젝트 문서
```

## 🌐 Global Access

- **로컬 접속**: `http://localhost:8000`
- **외부 접속**: `http://[IP주소]:8000`
- **글로벌 배포**: Vercel URL (자동 생성)

## 🔧 Configuration

### 환경별 설정
- **개발**: 로컬 서버 실행
- **테스트**: Vercel Preview 배포
- **프로덕션**: Vercel Production 배포

### 결제 설정
- **테스트**: Stripe 테스트 키 사용
- **실제**: Stripe 라이브 키로 교체

## 📱 Supported Browsers

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## 🔒 Security

- HTTPS 강제 적용 (Vercel)
- XSS 보호
- Content Security Policy
- Secure Headers

## 📞 Support

문제가 있으시면 언제든 연락주세요!

---

**Artificial NY** - 전 세계를 연결하는 AI 미술품 검증 서비스 