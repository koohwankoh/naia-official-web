# 주식회사 나이아 (NAIA Inc.) & 엔인공지능에이전트연구소 공식 웹사이트 배포 패키지 (v2.0)

- **가비아(Gabia) 결제 완료 공식 도메인**: `https://www.naia.kr` (보조 도메인: `naia.kr`, `naialab.co.kr`)
- **GitHub Pages 임시 스테이징 URL (오픈 전 확인용)**: `https://[사용자ID].github.io/naia-official-web/`
- **관리자(ADMIN) 전용 URL**: `https://www.naia.kr/admin.html` (또는 메인 화면 상단 `[⚙️ 관리자(ADMIN) 전환]` 버튼 클릭)

---

## 1. 7대 핵심 사업영역 카탈로그 구성
1. **NAIA소개**: AAA 핵심 철학(Artist, Architect, Agent), 5대 핵심가치, 전사 2본부 9부서 조직도 (v1.3 인포그래픽 탑재)
2. **AI트랜드, AI최신기술동행**: 웨이크업뉴스(Wakeup News) 기획특집 [AI퍼스트] (봇의 시대와 AI 워커, 프롬프트를 넘어 업무설계로, AI 브라우저 Aside vs Comet, 환각 검증 체계)
3. **AI교육, AI컨설팅**: G-AIGrapher 전문가 자격 양성 코스, 2026 생성형 AI 실전 마스터 과정(10주 완성), 기업 B2B AX 맞춤형 컨설팅 & 사내 보안 격리형 Private RAG
4. **AI출판, AI홍보, AIT뉴스**: 웨이크업뉴스 디지털 저널리즘 및 매일 아침 AIT 뉴스레터, 도서 출판 표준 SOP 기반 단행본 편찬 및 ISBN 등록, 보도자료/PR 자동화
5. **AI인문학, AI저술**: 웨이크업뉴스 기획연재 『만화로 배우는 천자문』(1~32화), 『도덕경 81장』 하이브리드 단행본, 생활문학 [노래로 즐기는 한국음식] 홍어찜 & 떡볶이 이야기, AI 자서전 집필
6. **AI음악, AI영상**: 나인빛TV (@ninebeat-s9u) 판소리·국악 x EDM/R&B/팝 K-Sound 81곡 프로젝트, Suno/Udio 기반 AI 작사·작곡, AI 시네마틱 영상
7. **건강·웰니스**: AI 기반 시니어 관절 건강 케어, 마인드 밸런스 수면 ASMR & 모닝 긍정 확언(Morning Positive Affirmation), 푸드 테라피 웰니스

---

## 2. GitHub Pages 임시 오픈 3단계 절차
1. **GitHub 저장소 생성**: GitHub(https://github.com) 로그인 후 `naia-official-web` 이름으로 Public Repository를 생성합니다.
2. **패키지 파일 업로드**: 본 ZIP 압축 해제 후 모든 파일(`index.html`, `admin.html`, `CNAME`, `assets/`, `.github/workflows/deploy.yml`)을 그대로 업로드하고 커밋합니다.
3. **GitHub Pages 활성화**:
   - 저장소 상단 `Settings` > 좌측 `Pages` 메뉴 이동
   - Build and deployment > Source를 `Deploy from a branch` (Branch: `main` / `/root`)로 선택
   - 약 1분 뒤 `https://[사용자ID].github.io/naia-official-web/` 임시 주소로 전 세계 어디서든 접속 가능합니다.

---

## 3. 가비아(Gabia) DNS 최종 연동 방법 (www.naia.kr)
임시 오픈 사이트 검토가 완료되면 가비아 콘솔에서 아래 레코드를 등록합니다:
1. **CNAME 레코드 추가**:
   - 호스트: `www`
   - 값/위치: `[사용자ID].github.io.`
2. **A 레코드 추가 (루트 도메인 naia.kr용 GitHub Pages IP 4개)**:
   - 호스트: `@` (또는 빈칸)
   - 값: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. GitHub 저장소 `Settings` > `Pages` > `Custom domain`에 `www.naia.kr`을 입력하고 `Enforce HTTPS`를 체크합니다.

---

## 4. 임시 관리자(ADMIN) 계정 안내
- **총괄 마스터 (대표이사·비서실)**: ID `naia_admin` / PW `NaiaLab@2026!`
- **개발·기술 관리자 (AI개발팀·기술팀)**: ID `dev_manager` / PW `AgentDev#2026`
- **홍보·미디어 관리자 (홍보실·영업팀)**: ID `pr_editor` / PW `WakeUp@2026`
