# 🔄 자동 복구 스크립트 (Auto Recovery Script)

## 신규 대화창에서 즉시 실행할 MCP 명령어

### 1단계: 프로젝트 상태 즉시 조회 (30초)
```typescript
// Task Master 상태 확인
get_tasks({
  projectRoot: "C:\\Users\\user2020-06\\Desktop\\glec-api-dev2",
  withSubtasks: true
});

// GitHub 리포지토리 상태 확인
get_file_contents({
  owner: "DEOKHOKANG",
  repo: "glec-api-platform-2025",
  path: ""
});

// Supabase 프로젝트 상태 확인
get_project({
  id: "xjxtwztyiebucistkejm"
});

// 지식 그래프 조회
read_graph();
```

### 2단계: 다음 작업 자동 결정 (10초)
```typescript
// 다음 우선순위 작업 확인
next_task({
  projectRoot: "C:\\Users\\user2020-06\\Desktop\\glec-api-dev2"
});

// 복잡도 분석 리포트
complexity_report({
  projectRoot: "C:\\Users\\user2020-06\\Desktop\\glec-api-dev2"
});
```

### 3단계: 컨텍스트 완전 복구 확인 (10초)
```typescript
// Postman 워크스페이스 확인 (Postman이 설정된 경우)
get-collections();

// Supabase 연결 키 재확인
get_anon_key({
  project_id: "xjxtwztyiebucistkejm"
});
```

## 📋 즉시 복구용 프로젝트 정보

### 핵심 식별자
- **Task Master 경로**: `C:\Users\user2020-06\Desktop\glec-api-dev2`
- **GitHub 리포지토리**: `DEOKHOKANG/glec-api-platform-2025`
- **Supabase 프로젝트 ID**: `xjxtwztyiebucistkejm`

### 현재 진행 상태
- **완료된 작업**: 1, 3 (13.33% 진행률)
- **다음 우선순위**: 작업 2 (API Gateway 구현)
- **의존성**: 작업 2는 작업 1 완료로 실행 가능

### 환경 설정 (로컬 개발용)
```bash
SUPABASE_URL=https://xjxtwztyiebucistkejm.supabase.co
SUPABASE_ANON_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InhqeHR3enR5aWVidWNpc3RrZWptIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NDgxNzYyMzAsImV4cCI6MjA2Mzc1MjIzMH0.Aw-APHb5MHgTEBMopaqJXpSCyS62sXbGJlCW5mjtICM
```

## 🚨 긴급 상황별 복구 가이드

### 상황 1: Task Master 데이터 손실
```typescript
// 프로젝트 재초기화
initialize_project({
  projectRoot: "C:\\Users\\user2020-06\\Desktop\\glec-api-dev2",
  yes: true
});

// PRD 기반 작업 구조 재생성
parse_prd({
  projectRoot: "C:\\Users\\user2020-06\\Desktop\\glec-api-dev2",
  input: "scripts\\prd.txt",
  numTasks: "15"
});

// 완료된 작업 상태 복구
set_task_status({
  id: "1,3",
  status: "done",
  projectRoot: "C:\\Users\\user2020-06\\Desktop\\glec-api-dev2"
});
```

### 상황 2: GitHub 연결 문제
```typescript
// 리포지토리 재연결 확인
get_file_contents({
  owner: "DEOKHOKANG",
  repo: "glec-api-platform-2025",
  path: "docs/PROJECT_CHECKPOINT.md"
});

// 최신 체크포인트 파일 확인
// 필요시 새 파일 추가
```

### 상황 3: Supabase 연결 문제
```typescript
// 프로젝트 상태 재확인
get_project({
  id: "xjxtwztyiebucistkejm"
});

// 데이터베이스 테이블 확인
list_tables({
  project_id: "xjxtwztyiebucistkejm"
});

// 연결 키 재발급 (필요시)
get_anon_key({
  project_id: "xjxtwztyiebucistkejm"
});
```

## ✅ 복구 검증 체크리스트

### 기본 검증
- [ ] Task Master 작업 목록 정상 로드 (15개 작업)
- [ ] GitHub 리포지토리 파일 접근 가능
- [ ] Supabase 프로젝트 ACTIVE_HEALTHY 상태
- [ ] 지식 그래프 프로젝트 엔티티 존재

### 상세 검증
- [ ] 작업 1, 3 완료 상태 확인
- [ ] 다음 작업 2 실행 가능 상태
- [ ] database.ts 타입 파일 존재 확인
- [ ] 환경 변수 키 유효성 확인

### 완전 복구 확인
- [ ] 모든 MCP 도구 연결 정상
- [ ] 프로젝트 진행률 13.33% 표시
- [ ] 다음 액션 자동 제시 기능 작동

---

**이 스크립트를 사용하여 어떤 상황에서도 50초 이내에 프로젝트 컨텍스트를 완전 복구할 수 있습니다.**