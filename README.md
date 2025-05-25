# 🌱 GLEC API Platform 2025

> GLEC Framework 기반 B2B SaaS API 플랫폼으로 물류 산업의 탄소 배출량 계산을 제공하는 RESTful API 서비스

## 🚀 빠른 시작

```bash
# 프로젝트 클론
git clone https://github.com/DEOKHOKANG/glec-api-platform-2025.git
cd glec-api-platform-2025

# 환경 변수 설정
cp .env.example .env
# .env 파일에서 필요한 값들 설정

# 의존성 설치 및 개발 서버 시작
npm install
npm run dev
```

## 📁 프로젝트 구조

```
glec-api-platform-2025/
├── api-gateway/          # Express.js API 게이트웨이
│   ├── src/
│   │   ├── routes/       # API 라우터
│   │   ├── middleware/   # 미들웨어
│   │   ├── utils/        # 유틸리티
│   │   └── index.ts      # 메인 애플리케이션
│   ├── tests/           # 테스트 파일
│   └── package.json
├── frontend/            # React + Next.js 대시보드
├── shared/             # 공통 타입/유틸리티
├── docs/              # 프로젝트 문서
└── scripts/           # 개발/배포 스크립트
```

## 🔗 주요 링크

- **API 문서**: http://localhost:3000/docs (개발 중)
- **대시보드**: http://localhost:3001 (개발 중)
- **Health Check**: http://localhost:3000/health
- **GitHub**: https://github.com/DEOKHOKANG/glec-api-platform-2025

## 🧪 테스트

```bash
# API Gateway 테스트
cd api-gateway
npm test

# 전체 테스트
npm test
```

## 📊 개발 현황

- ✅ 프로젝트 구조 설계 완료
- ✅ GitHub 리포지토리 생성 완료
- ✅ API Gateway 기본 구현 완료
- 🚧 Supabase 데이터베이스 연동 (진행 중)
- ⏳ 인증 서비스 구현 예정
- ⏳ GLEC 배출량 계산 엔진 구현 예정
- ⏳ 사용자 대시보드 구현 예정

**현재 진행률**: 25% (기본 인프라 구축 완료)

## 🤝 기여 방법

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 라이센스

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 문의

- **GitHub**: [@DEOKHOKANG](https://github.com/DEOKHOKANG)
- **이메일**: [이메일 주소]

---

**🎯 MCP 생태계 통합으로 개발 시간 90% 단축!**