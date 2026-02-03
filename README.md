# n8n-workflw

남들이 못 하는 기술을 활용하여 대중이 원하는 결과물을 가장 쉽게 만드는 강사, 후츠릿의 AI 자동화 시스템 저장소입니다. 이 저장소의 모든 기록은 AI 에이전트를 통해 구조화되고 자동으로 관리됩니다. 실무에 즉시 적용 가능한 워크플로우와 코드를 보관합니다.

### 시스템 구조

해당 저장소는 다음과 같은 구조로 운영됩니다. 모든 파일명은 케밥 케이스(kebab-case)를 준수합니다.

```text
.
├── workflows/              # n8n 워크플로우 JSON 파일 저장소
│   ├── ai-agents/          # LLM, LangChain, 에이전틱 워크플로우 기반 지능형 자동화
│   ├── data-processing/    # 웹 스크래핑, 데이터 정제 및 변환 자동화 로직
│   ├── marketing/          # 블로그, 링크드인, SNS 콘텐츠 생성 및 자동 배포 시스템
│   └── utility/            # 정보 수집, 알림, 시스템 관리용 보조 워크플로우
├── scripts/                # n8n Code Node 전용 외부 스크립트
│   ├── python/             # Python 3.11+ 기반 처리 로직 (Type Hinting 적용)
│   └── javascript/         # JSON 가공 및 프론트엔드 연동용 JS 코드
├── docs/                   # 아키텍처 설계도, 기술 규격서 및 API 연동 명세서
├── templates/              # 수강생 및 독자 배포용 입문자용 초급 템플릿
├── etc/                    # 비정형 참고 자료 및 자산
│   ├── images/             # n8n 캔버스 캡처 및 블로그용 시각 자료
│   ├── references/         # 기술적 영감을 준 외부 워크플로우 및 링크 모음
│   └── drafts/             # 로직 설계 초안 및 API 응답 샘플(JSON)
├── .gitignore              # API Key 및 민감한 환경 변수 제외 설정
└── README.md               # 저장소 전체 현황 및 운영 전략 기록
```

### 기술적 사양 및 환경

본 저장소의 워크플로우와 코드는 다음 환경에서 최적화되었습니다.

- **하드웨어**: M1 MacBook Air (고사양 작업 시 Google Colab 연동)
- **런타임**: n8n (Self-hosted or Cloud), Python 3.11+
- **주요 도구**: OpenAI API, LangChain, MongoDB, Vector Databases
- **자동화 핵심**: n8n의 Git Node를 통한 실시간 변경 사항 자동 동기화 및 README 업데이트
