# SEDNA BRAND FILM — "DON'T SEARCH. EXPLORE."
### 최종 홍보영상 기획서 · 연출 콘티 · 제작 가이드 (Production Bible v1.0)

> 러닝타임: **1:55** (픽처 락) + 3초 음악 테일 = 1:58
> 포맷: 3840×2160 / 24fps / 2.39:1 레터박스(UI 컷은 16:9 안에 배치) / 컬러 Rec.709 (HDR 마스터는 선택)
> 제작 방식: 실제 SEDNA 화면 + 3D(Blender/Three.js) + AI 영상 플레이트 + After Effects 합성

> **참고 메모** — 레퍼런스 영상(YouTube 3v9X3ufzBnQ)은 이 환경에서 직접 시청하지 못했습니다. 본 기획은 요청서에 기술된 서사 구조(암흑 → 지구 → 접근 → 탐사 → 발견 → 브랜드)를 기준으로 독립 구성했으며, 레퍼런스의 화면·대사는 사용하지 않습니다. 레퍼런스의 리듬/톤을 맞추고 싶다면 편집자가 시청 후 §9 "튜닝 포인트"만 조정하세요.

---

## 0. 한 장 요약

| 항목 | 내용 |
|---|---|
| 로그라인 | 모두가 결과를 *검색*할 때, 한 탐사선이 시장 전체를 *탐사*하고, 아무도 보지 못한 빈 공간에서 새로운 별을 발견한다. |
| 핵심 은유 | 검색 결과 = 이미 밝혀진 별 / 시장 공백 = 아직 발견되지 않은 별 |
| 컬러 규칙 | 영상 전체가 **블루·블랙 단색 세계**. 유일한 **웜 컬러(앰버)** 는 *MARKET GAP / OPPORTUNITY* 에서만 등장 → "기회 = 따뜻한 빛" |
| 연출 원칙 | 컷 편집 최소화, **한 번의 카메라 여정**. 전환은 모두 카메라 이동·매치무브·디졸브로 처리 |
| 금지 | 글리치, 네온, 렌즈플레어 남발, 게임 HUD, 자막 폭주, 스톡 SaaS 제스처(손가락 터치/노트북 든 사람) |
| 비율 | 브랜드(우주/3D/AI/타이포) ≈ 50% · 실제 UI ≈ 50% — §8 참조 |

---

## 1. 스타일 바이블

### 1-1. 컬러 토큰
| 이름 | HEX | 용도 |
|---|---|---|
| VOID | `#02040A` | 배경 기본 |
| DEEP | `#07111F` | UI 패널 배경 |
| ORBIT BLUE | `#0B2A4A` | 대기권, 그림자 블루 |
| SIGNAL | `#5BA8FF` | 데이터 라인, 핀, 주요 텍스트 강조 |
| FROST | `#DCEBFF` | 본문 텍스트, 타이틀 |
| GAP AMBER | `#FFC56B` | **시장 공백·기회 전용 (다른 곳 사용 금지)** |

### 1-2. 타이포
- 영문 타이틀: **Neue Montreal / Söhne / Inter Tight** Light~Regular, 자간 +180~+300, 전부 대문자
- 데이터/상태값: **IBM Plex Mono / JetBrains Mono** 11~14px 상당, 불투명도 60~80%
- 한글: **Pretendard** Light/Regular (나레이션 자막·키워드)
- 타이틀 크기: 화면 높이의 **4~5%**. 크게 쓰지 않는다. 등장은 *페이드 + 자간 0.6초 확장*.

### 1-3. 모션 룰
- 이징: 모든 이동 `cubic-bezier(0.22, 0.0, 0.0, 1.0)` 계열(아주 느린 시작 + 긴 감속)
- 텍스트 인/아웃 각각 **0.8초**, 등장 시 블러 6px→0
- 스캔라인은 **수평 1px 라인 + 잔광 0.5초**, 색은 SIGNAL 또는 (GAP 장면에서) AMBER
- 카메라에는 **미세한 핸드헬드 대신 "위성 드리프트"**: 0.3% 스케일의 초저속 흔들림

### 1-4. 탐사선 "NEW HORIZONS" 디자인 (오리지널 가이드)
실제 NASA 탐사선의 로고·형태를 그대로 복제하지 않고, *골드 포일 바디 + 흰색 고이득 안테나 접시 + 길게 뻗은 붐* 정도의 **일반적 딥스페이스 프로브 문법**으로 오리지널 디자인한다.
**NASA 로고/미션 패치/실제 텍스트 사용 금지.** "NEW HORIZONS"는 SEDNA 엔진명으로만 사용(상표·홍보 사용 범위는 배포 전 법무 확인 권장).

---

## 2. 전체 구조 한눈에 (컷 31개)

| Scene | 구간 | 컷 | 성격 |
|---|---|---|---|
| 01 THE UNKNOWN MARKET | 0:00–0:12 | C01–C03 | 브랜드(AI/3D) |
| 02 THE QUESTION | 0:12–0:25 | C04–C06 | 브랜드(3D+AI+AE) |
| 03 MISSION START | 0:25–0:38 | C07–C10 | 브랜드 → UI 전환 |
| 04 SCANNING MARKET | 0:38–0:55 | C11–C14 | 실제 UI(3D 지구본·지도) |
| 05 THE ENGINE | 0:55–1:12 | C15–C18 | 실제 UI + AE 오버레이 |
| 06 MARKET GAP | 1:12–1:30 | C19–C22 | **하이라이트** (UI → 브랜드 화) |
| 07 OPPORTUNITY | 1:30–1:43 | C23–C26 | 브랜드 + 실제 UI |
| 08 HORIZON | 1:43–1:55 | C27–C31 | 브랜드 |

**제작 태그 범례**
- 🟦 `[REAL]` 실제 SEDNA 화면 녹화 필요
- 🟪 `[AI]` AI 영상 생성(Kling/Veo/Sora/Runway)
- 🟧 `[AE]` After Effects 제작
- 🟩 `[3D]` Blender 또는 Three.js 제작

---

## 3. 상세 콘티 (컷 단위)

표기: **TC**(타임코드) · **화면** · **카메라** · **텍스트(KO/EN)** · **나레이션** · **SFX** · **BGM** · **전환** · **제작**

---

### SCENE 01 — THE UNKNOWN MARKET (0:00–0:12)
**BGM M1 "VOID"** — D 마이너 드론, 무박(무리듬), 하이패스된 딥 패드. 0:00 무음 → 0:01 서브 럼블 페이드인.

#### C01 · 0:00.0–0:03.0 · 완전한 암흑
- **화면**: 순수 블랙. 0:01.5부터 극소수의 별이 한 개씩 떠오른다(3→40개). 별은 크기·밝기 편차가 크고 일부는 미세하게 깜빡임.
- **카메라**: 고정 → 아주 느린 전진 시작(Z축 +0.5%/s).
- **텍스트**: 없음
- **나레이션**: 없음
- **SFX**: Deep Space Rumble(28–40Hz 서브, 페이드인), 0:02.3 아주 작은 Satellite Signal 1회(먼 곳에서 온 것 같은 사인 핑)
- **BGM**: M1 시작
- **전환**: 이어짐(연속 플레이트)
- **제작**: 🟪 `[AI]` 또는 🟩 `[3D]` (별 필드는 Blender/AE Particular 로도 충분)

#### C02 · 0:03.0–0:07.0 · 지구의 림(Limb) 등장
- **화면**: 별밭 하단에서 **지구의 곡선이 빛나는 가장자리(림)** 로 먼저 나타난다. 태양은 프레임 밖 좌측 상단. 대기권 블루 글로우가 얇게 번짐.
- **카메라**: 느린 **dolly-in + 미세 tilt up**. 지구가 프레임 하단 35% 차지.
- **나레이션**: 0:03.5 *"우리가 매일 검색하는 인터넷에는 / 수없이 많은 정보가 존재합니다."*
- **SFX**: 대기 저역 스웰(Low swell), 별 반짝임 마이크로 틱 없음(과잉 금지)
- **BGM**: 드론에 고음 글래스 패드 1음 추가
- **전환**: 연속
- **제작**: 🟪 `[AI]` 메인 + 🟩 `[3D]` 대체안(Blender Earth)

#### C03 · 0:07.0–0:12.0 · 회전하는 지구 · 타이틀
- **화면**: 지구가 프레임 중앙으로 올라와 **고해상도로 천천히 자전**(동→서 흐름이 아닌 실제 자전 방향). 야간면에 도시 불빛이 희미하게 보이기 시작.
- **카메라**: dolly-in 지속. 마지막 1초에 약간의 감속.
- **텍스트**: 0:09.0 하단 중앙 작게 **`THE UNKNOWN MARKET`** (영화 타이틀처럼 페이드 + 자간 확장), 0:11.3 페이드아웃
- **나레이션**: 0:05.8 *"검색량."* (0.7s 쉼) *"콘텐츠."* (0.7s) *"경쟁자."* (0.9s) *"그리고 아직 아무도 발견하지 못한 기회."* (→ 0:12.2까지)
- **SFX**: 각 단어마다 **아주 작은 Digital Ping**(단어 끝에 -24dB), 마지막 문장에서 Sub Bass 한 번 낮게
- **BGM**: 패드 상승, 아직 리듬 없음
- **전환**: 지구를 향한 카메라 이동이 그대로 S02로 이어짐
- **제작**: 🟪 `[AI]` 또는 🟩 `[3D]`, 타이틀 🟧 `[AE]`

---

### SCENE 02 — THE QUESTION (0:12–0:25)
#### C04 · 0:12.0–0:16.5 · 대한민국 접근 · 데이터 포인트
- **화면**: 지구가 화면을 가득 채우며 아시아 → 한반도로 접근. 야간면 도시 불빛. **서울·부산·대구·경주·포항**에 작은 포인트가 별처럼 하나씩 켜지고, 포인트 사이를 **머리카락 두께의 곡선 라인**이 연결(호 형태, 아주 옅음). 지명은 **포인트 옆에 작게** `SEOUL` `BUSAN` `DAEGU` `GYEONGJU` `POHANG`(Mono, 10px 상당).
- **카메라**: 지구 곡률이 서서히 평평해지는 **느린 dolly + 경사 각도 55° → 70°**
- **나레이션**: 0:12.8 *"하지만 우리는 / 그 대부분을 발견하지 못한 채 지나칩니다."*
- **SFX**: 포인트 점등마다 Digital Ping(각기 다른 음정, 저음), Satellite Whoosh(저역) 1회
- **BGM**: 패드 유지, 저역 펄스 진입 전 "숨" 구간
- **전환**: 카메라 계속 이동
- **제작**: 🟩 `[3D]` 지구/지형·라인, 🟧 `[AE]` 라벨/포인트, (플레이트 대체) 🟪 `[AI]`

#### C05 · 0:16.5–0:18.5 · 정적
- **화면**: 포인트 광량 -60%, 라인만 호흡하듯 천천히 깜빡. 한반도 전체가 조용히 떠 있음.
- **카메라**: 거의 정지(0.2%/s 드리프트만)
- **나레이션**: 없음 — **2초 정적 (이 영상의 첫 번째 숨)**
- **SFX**: 서브 럼블만. 모든 고역 제거
- **BGM**: 패드 페이드 -10dB
- **전환**: 이어짐
- **제작**: 🟩 `[3D]` + 🟧 `[AE]`

#### C06 · 0:18.5–0:25.0 · 질문 · 탐사선 등장
- **화면**: 한반도 위 공간에서 화면 중앙에 **아주 작은 탐사선 실루엣**이 별빛을 받으며 나타난다. 대한민국의 포인트들이 탐사선 쪽으로 미세하게 "끌리는" 느낌(라인이 탐사선 방향으로 약 3° 휘어짐).
- **카메라**: 탐사선 뒤쪽 로우앵글에서 **slow push-in**
- **텍스트**: 0:23.0 **`NEW HORIZONS`** (탐사선 옆 작은 라벨), 0:24.0 중앙 하단 **`NEW HORIZONS ENGINE`** 타이틀
- **나레이션**: 0:18.8 *"그렇다면,"* (0.6s) *"이 거대한 데이터 속에서"* *"우리가 원하는 시장만"* *"탐사할 수 있다면 어떨까요?"*
- **SFX**: 탐사선 등장 시 Low Frequency Impact(약하게, -12dB), 미세 Satellite Signal 3회
- **BGM**: M1 → 0:22.5부터 **M2 "SIGNAL"** 예고 — 저역 펄스 60 BPM 페이드인
- **전환**: 탐사선 엔진 글로우가 켜지며 S03으로
- **제작**: 🟩 `[3D]` 탐사선 모델, 🟪 `[AI]` 탐사선 히어로 플레이트, 🟧 `[AE]` 타이틀/라벨

---

### SCENE 03 — MISSION START (0:25–0:38)
**BGM M2 "SIGNAL"** — 펄스 72 BPM, 서브 베이스 플럭, 하이햇 없음, 얇은 아르페지오(16분음표 대신 8분음표 2개마다 1회).

#### C07 · 0:25.0–0:29.0 · 탐사선 → 지구
- **화면**: 탐사선이 카메라 앞을 가로질러 지구를 향해 천천히 이동. 엔진(이온 스러스터)의 **차가운 블루 글로우**. 골드 포일이 지구 반사광을 받음.
- **카메라**: 탐사선 뒤따르는 **tracking shot**, 아주 미세한 roll +0.5°
- **나레이션**: 0:26.0 *"우리는 이 탐사를 위해 / 하나의 시스템을 만들었습니다."*
- **SFX**: Satellite Whoosh(저역 중심), 스러스터 저주파 허밍
- **BGM**: 펄스 진입, 아르페지오 첫 음
- **전환**: 탐사선이 대기권에 닿을 즈음 **지구 대기 곡선이 UI 배경의 곡선으로 매치**
- **제작**: 🟩 `[3D]` 또는 🟪 `[AI]` + 🟧 `[AE]`

#### C08 · 0:29.0–0:31.0 · 우주 → UI 전환 (시그니처 전환)
- **화면**: 카메라가 대기권 **안개 같은 블루** 속으로 진입 → 프레임 전체가 블루 그라디언트 → 그 블루가 **SEDNA 검색 화면의 배경 그라디언트로 그대로 이어짐**. (중간에 흰 플래시 금지)
- **카메라**: 전진 지속 → 5프레임 동안 모션 블러 포함 → UI 안착 시 정지
- **SFX**: 대기 진입 Whoosh(필터 스윕 저→고) → UI 안착 시 Sub Bass Hit
- **BGM**: 펄스 유지
- **전환**: 대기권 컬러(#0B2A4A→#07111F) 그라디언트 **매치 디졸브** (에디터: 두 플레이트의 중앙 픽셀 색을 동일하게 맞춘 후 12프레임 크로스디졸브)
- **제작**: 🟧 `[AE]` 전환 합성

#### C09 · 0:31.0–0:36.0 · SEDNA 검색창
- **화면**: SEDNA 검색 UI가 중앙에 **작게(화면 폭의 40%)** 등장. 필드 2개: `지역` → **경주** 타이핑, `업종` → **숙소** 타이핑. 입력 중 미세한 커서 깜빡임. 배경에는 살짝 흐린 지구 실루엣이 남아 있음.
- **카메라**: UI를 향해 **3% 스케일 slow push**, 타이핑 속도는 자연스러운 사람 속도 × 0.8
- **텍스트(UI)**: `지역` `경주` / `업종` `숙소` / 버튼 `탐사 시작`
- **나레이션**: 0:32.0~0:35.0 무음(타이핑 소리만) — *여기서 나레이션이 쉬어야 시청자가 UI를 읽는다*
- **SFX**: 키입력은 일반 키보드가 아니라 **아주 작은 Digital Ping 패밀리 + 기계적 "tick"** (음정 낮음, -22dB). 버튼 호버 시 Radar Scan 미세음
- **BGM**: 펄스 + 아르페지오 지속
- **전환**: 버튼 위로 커서 이동 → C10
- **제작**: 🟦 `[REAL]` (필드 입력 시퀀스 녹화) + 🟧 `[AE]` (글로우/배경 합성)

#### C10 · 0:36.0–0:38.0 · MISSION START
- **화면**: 버튼 클릭 → 버튼 테두리에서 **얇은 링 펄스** 한 번 퍼짐 → 배경 지구가 살짝 밝아짐. 화면 중앙 **`MISSION START`** 텍스트.
- **텍스트**: **`MISSION START`** (0:36.4~0:38.0)
- **나레이션**: 0:36.0 *"SEDNA."* (낮게, 단독)
- **SFX**: **클릭음 = 탐사 장비 잠금 해제음**(금속성 "thunk" + 저역 Low Frequency Impact -10dB + 짧은 Radar Scan), 클릭 직후 0.3s 무음
- **BGM**: **텐션 상승 → 0:38 드롭 없이 리듬 증가(하이햇 진입, 90 BPM)**
- **전환**: 지구가 화면 안으로 빨려 들어가듯 줌 시작 → S04
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]`

---

### SCENE 04 — SCANNING MARKET (0:38–0:55)
**BGM M3 "DESCENT"** — 90 BPM, 서브 베이스 + 얇은 펄스, 탐사 중 "착륙" 감각.

#### C11 · 0:38.0–0:43.0 · 우주 → 지구 → 대한민국
- **화면**: SEDNA 3D 지구본 화면. 우주에서 지구를 보다가 **한반도로 접근**. 경계선·해안선은 SIGNAL 블루 1px, 배경은 위성 텍스처(어둡게).
- **카메라**: 위성 카메라 같은 **S자 완만한 곡선 이동**, 과도한 줌 금지 → ease-in-out 5초
- **텍스트(화면)**: 좌하단 Mono 소형 `ORBIT 35,786 KM` → `KOREA` 에서 `ALT 620 KM` 로 카운트 다운 (장식용, 불투명도 50%)
- **나레이션**: 0:38.6 *"SEDNA는 지역을 탐색하고 / 시장을 스캔합니다."*
- **SFX**: Satellite Whoosh(저역), 고도 수치가 바뀔 때 미세한 Digital Ping
- **BGM**: 드롭 없이 볼륨 +3dB
- **전환**: 연속
- **제작**: 🟦 `[REAL]` (Three.js 지구본 녹화) + 🟩 `[3D]`(보강용 별 배경/대기) + 🟧 `[AE]`(고도 텍스트)

#### C12 · 0:43.0–0:47.0 · 경상북도 → 경주
- **화면**: 한반도 → 경상북도 → **경주**로 접근. 행정 경계가 얇은 라인으로 부드럽게 나타났다 사라짐. 경주에 닿으면 점이 하나 켜짐.
- **카메라**: 지표면 각도로 경사 하강 (피치 70° → 45°)
- **텍스트**: `GYEONGBUK` → `GYEONGJU` (Mono 12px, 좌하단 → 포인트 옆으로 이동)
- **나레이션**: 0:43.4 *"검색 결과를 보는 것이 아니라"*
- **SFX**: 행정 경계가 그려질 때 Radar Scan 미세음 (1회)
- **BGM**: 동일
- **전환**: 위성 타일이 **지도 타일로 모프**(C13)
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]`

#### C13 · 0:47.0–0:51.0 · 지도 전환 · 핀 01~10
- **화면**: 위성 이미지가 SEDNA **지도 화면**으로 전환. 경주 시내/황리단길/터미널/보문 권역 중심. **핀 01→10** 이 0.25초 간격으로 순차 생성. 각 핀 생성 시 작은 원형 리플 1회.
- **카메라**: 지도는 **3% 줌인 + 5° 틸트**로 생동감
- **텍스트**: 핀 숫자 `01`…`10` (Mono)
- **나레이션**: 0:47.3 *"시장이 어떻게 움직이고 있는지를 / 추적합니다."*
- **SFX**: 핀마다 Digital Ping (피치 점차 상승, 10개째에서 옥타브 업), 마지막 핀에 Low Frequency Impact 약하게
- **BGM**: 아르페지오 상승
- **전환**: 10번 핀 등장 후 연속
- **제작**: 🟦 `[REAL]` 지도+핀 녹화 + 🟧 `[AE]` 리플 강화

#### C14 · 0:51.0–0:55.0 · SCANNING MARKET
- **화면**: 지도 위에 **수평 스캔 링(레이더 웨이브)** 이 중심에서 퍼져나가며 핀마다 작은 카드가 뜬다(블로그 제목 + 순위 숫자). 스캔 링이 끝에 닿으면 화면이 한 톤 어두워지며 분석 패널로 이어짐.
- **텍스트**: **`SCANNING MARKET`** (0:51.5~0:54.0, 좌상단 작게)
- **나레이션**: 없음 (0:52~0:55 정적 — 스캔음만)
- **SFX**: Radar Scan (스윕 3초), 카드 생성 Digital Ping
- **BGM**: 릴리즈 없이 유지, 하이햇 가벼움
- **전환**: 지도 그레이딩 다운 → 패널이 위로 **slide-fade**
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]`

---

### SCENE 05 — THE ENGINE (0:55–1:12)
**BGM M4 "ANALYSIS"** — 96 BPM, 펄스 + 글리치 없는 미세 퍼커션(얇은 클릭), 점점 밀도 증가.

#### C15 · 0:55.0–0:59.0 · 엔진 가동
- **화면**: 어두운 공간 중앙에 **NEW HORIZONS ENGINE** 코어(얇은 원형 링 2개 + 중앙 타이포). 링이 천천히 반대 방향으로 회전. 상태값이 좌하단에서 교체: `ANALYZING…` → `SCANNING…` → `PROCESSING…`
- **카메라**: 코어를 향한 slow dolly-in (2%)
- **텍스트**: 중앙 **`NEW HORIZONS ENGINE`**, 주변에 12개 항목이 *차례로* 스쳐감(한 화면에 4개 이하 동시 노출): `TOP CONTENT` `TOP 10` `KEYWORD` `COMPETITOR` `PLACE` `SEARCH INTENT` `CONTENT LENGTH` `IMAGE` `BLOG` `LOCAL SEARCH` `KEYWORD FREQUENCY` `CONTENT STRUCTURE`
- **나레이션**: 0:55.5 *"SEDNA의 뉴호라이즌스 엔진은 / 수많은 데이터를 하나씩 분석합니다."*
- **SFX**: Data Processing(저역 스트림), 링 회전 미세 모터음, 항목 스침마다 Digital Ping(-28dB)
- **BGM**: 밀도 증가 시작
- **전환**: 링이 확장되어 패널 그리드로 변환
- **제작**: 🟧 `[AE]` (엔진 코어/키워드 스침) + 🟦 `[REAL]`(상태값 패널 참조)

#### C16 · 0:59.0–1:03.0 · TOP 콘텐츠 카드
- **화면**: SEDNA **상위 콘텐츠 TOP10 리스트**가 카드형으로 펼쳐짐. 각 카드: 순위 / 제목 / 글자수 / 이미지 수. **글자수 막대**가 좌→우로 자라난다.
- **카메라**: UI를 **살짝 3D 공간에 띄운 느낌**(Z축 미세 패럴랙스), 카드가 카메라 쪽으로 **1cm씩 떠오르는** 느낌
- **텍스트**: `TOP CONTENT` `CONTENT LENGTH` `IMAGE`
- **나레이션**: 1:00.3 *"어떤 콘텐츠가 상위에 있는지."*
- **SFX**: 카드 넘김 Low tick, 막대 성장 Data Processing 사운드 업
- **BGM**: 밀도 +
- **전환**: 카드가 뒤로 밀리며 다음 패널
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]` 패럴랙스

#### C17 · 1:03.0–1:07.0 · 키워드·경쟁자·플레이스
- **화면**: **키워드 빈도** 차트(가로 막대가 아닌 *점 구름* 형태 권장), 경쟁 블로그 목록, 네이버 플레이스 관련 정보. 우측에 경쟁자 블로그 썸네일이 얇은 프레임으로 정렬.
- **카메라**: 수평 pan 1.5% → 패널 전환
- **텍스트**: `KEYWORD FREQUENCY` `COMPETITOR` `PLACE` `BLOG`
- **나레이션**: 1:04.0 *"경쟁자는 무엇을 이야기하고 있는지."*
- **SFX**: Digital Ping + 미세한 Radar Scan
- **BGM**: 동일
- **전환**: 패널 수평 슬라이드
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]`

#### C18 · 1:07.0–1:12.0 · 검색 의도 · 구조 → 별자리로 확산
- **화면**: **검색 의도(정보/비교/예약)** 클러스터와 **콘텐츠 구조(H2 구조, 이미지 수)**. 마지막 1.5초, UI가 **투명도 20%**까지 내려가며 키워드·경쟁 콘텐츠가 *점(별)* 이 되어 공간에 흩어진다 → S06 별자리 지도로 이어짐.
- **카메라**: pull-back 3%, 깊이감 증가 (DOF 얕게)
- **텍스트**: `SEARCH INTENT` `CONTENT STRUCTURE`
- **나레이션**: 1:08.0 *"사람들은 무엇을 찾고 있는지."*
- **SFX**: 저역 스웰 상승(riser), 마지막 0.5초에 모든 SFX 컷
- **BGM**: 펄스 상승 → **1:11.5 갑자기 볼륨 -12dB** (다음 장면 임팩트 준비)
- **전환**: UI → 점 구름 전환 (AE에서 UI 스크린샷의 **텍스트를 점으로 픽셀 분해**)
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]`(분해 전환) + 🟩 `[3D]`(점구름)

---

### SCENE 06 — MARKET GAP (1:12–1:30) ★ 핵심 장면
**BGM M5 "THE VOID"** — 1:12부터 저역 드론만. 펄스 제거. 1:21–1:23 완전 정적 → **1:23.0 임팩트**.

#### C19 · 1:12.0–1:17.0 · 별자리 같은 시장
- **화면**: 공간에 **경쟁 콘텐츠·키워드가 성단(클러스터)** 으로 떠 있다. 각 점은 블로그 글·키워드. 큰 클러스터가 몇 개, 그 사이에 **어두운 틈(void)** 이 존재한다. 점들은 SIGNAL 블루. UI 프레임은 거의 사라진 상태.
- **카메라**: 성단 사이로 **천천히 전진**하는 탐사선 POV
- **텍스트**: 없음 (집중)
- **나레이션**: 1:12.6 *"하지만 SEDNA가 찾는 것은 / 이미 존재하는 데이터만이 아닙니다."*
- **SFX**: 저역 드론, 먼 곳에서 들려오는 Satellite Signal 2회
- **BGM**: 드론
- **전환**: 카메라가 void 쪽으로 틸트
- **제작**: 🟩 `[3D]` (Blender/Three.js 점구름) + 🟧 `[AE]` + (옵션) 🟪 `[AI]` 배경 성운

#### C20 · 1:17.0–1:21.0 · 비어 있는 영역
- **화면**: 카메라가 성단들 사이의 **어두운 공백 영역**을 향해 전진. 공백 주변의 점들은 **그 영역을 피하듯** 배치되어 있음. 공백은 완전한 검정이 아니라 *아주 미세한 잔광*이 있다.
- **카메라**: 공백 중심으로 **slow push-in**, 페이스가 갈수록 느려짐
- **나레이션**: 1:17.6 *"경쟁자가 놓친 영역."* (0.6s) *"아직 충분히 다뤄지지 않은 검색어."*
- **SFX**: 저역 럼블 상승, Radar Scan 매우 멀리서 1회
- **BGM**: 드론 + 고역 -6dB
- **전환**: 동일 공간에서 스캔 시작
- **제작**: 🟩 `[3D]` + 🟧 `[AE]`

#### C21 · 1:21.0–1:24.0 · 스캔 라인 → IMPACT → MARKET GAP DETECTED
- **화면**: 1:21.0 **완전 정적 2초**(모든 소리 제거, 공백만 보임). 1:22.0 좌측에서 **가느다란 스캔 라인(수직 1px, SIGNAL)** 이 천천히 우측으로 이동. 라인이 공백을 지나는 순간(1:23.0) **AMBER 빛으로 바뀌며** 공백 영역이 테두리 라인으로 강조됨. 동시에 `MARKET GAP DETECTED`.
- **텍스트**: **`MARKET GAP DETECTED`** (1:23.0 등장, 자간 +300, 공백의 위쪽 배치, AMBER)
- **나레이션**: 1:22.6 *"바로,"* (쉼 1.0s)
- **SFX**: 스캔 라인 **Radar Scan(점진 고조)** → 1:23.0 **Deep Cinematic Boom + Sub Bass Hit + Low Frequency Impact** 3중 레이어, 이어서 1.5초 릴리즈 테일
- **BGM**: 1:21 정적 → 1:23 임팩트 후 드론이 **AMBER 색에 대응하는 따뜻한 패드(메이저 3도)** 로 전환
- **전환**: 카메라 고정 유지 (컷 없음)
- **제작**: 🟧 `[AE]` (스캔 라인/텍스트/AMBER 하이라이트) + 🟩 `[3D]`

#### C22 · 1:24.0–1:30.0 · 롱테일 키워드 발견
- **화면**: 공백 영역 안에서 **롱테일 키워드가 별처럼 하나씩** 켜진다. 6개를 0.8초 간격으로: `경주 터미널 근처 숙소` `황리단길 도보 숙소` `경주 외국인 숙소` `경주 조식 숙소` `경주 버스터미널 숙소` `경주 정원 숙소`. 각 키워드 옆에 작은 `LOW COMPETITION` 마커(Mono) 선택. 마지막 1초: `경주 터미널 근처 숙소` 가 **약간 더 크고 밝게** 강조.
- **카메라**: 공백 중심으로 **아주 느린 원호 궤도 이동**(orbit 6°)
- **텍스트**: 키워드 6개(한글 Pretendard 18px 상당), 영문 보조 `LONG-TAIL KEYWORD` 하단 작게
- **나레이션**: 1:24.0 *"시장에 남아 있는 / 빈 공간입니다."*
- **SFX**: 키워드마다 **고음 Digital Ping**(따뜻하고 맑은 벨 톤) + 작게 Satellite Signal
- **BGM**: 따뜻한 패드 지속, 피아노 싱글 노트 모티프(테마) 6음 → 키워드와 동기
- **전환**: 마지막 키워드의 빛이 폭발하지 않고 **한 점으로 수렴**
- **제작**: 🟧 `[AE]` + 🟩 `[3D]` + 🟦 `[REAL]` (실제 SEDNA의 롱테일 결과 화면은 C24에서 사용)

---

### SCENE 07 — OPPORTUNITY FOUND (1:30–1:43)
**BGM M6 "FOUND"** — 앰버 패드 상승, 펄스 재진입(84 BPM), 피아노 모티프 + 스트링 스웰.

#### C23 · 1:30.0–1:33.0 · 새로운 별의 탄생
- **화면**: 공백에 수렴한 빛이 **새로운 별 하나**로 응축되어 점점 밝아진다. 화면에서 유일한 따뜻한 광원. 주변 블루 성단이 그 빛에 미세하게 물든다(블루 → 블루 + 앰버 림).
- **카메라**: star를 향해 천천히 전진 → 별 주변에 작은 회절 링(렌즈플레어 금지, 링만)
- **텍스트**: **`OPPORTUNITY FOUND`** (1:30.8 등장)
- **나레이션**: 없음 (텍스트와 음악으로 전달)
- **SFX**: 저역 스웰 → 별 점등 시 Digital Ping(맑고 길게), Sub Bass 지속
- **BGM**: **상승** — 스트링 스웰 + 펄스 재진입
- **전환**: 별이 확대되며 SEDNA 결과 화면의 **AMBER 포인트**로 매치 컷
- **제작**: 🟪 `[AI]` 또는 🟩 `[3D]` + 🟧 `[AE]`

#### C24 · 1:33.0–1:38.0 · 탐사 결과 화면
- **화면**: 탐사 결과 화면이 깔끔하게 열린다. 패널 6개가 순차 등장: `추천 키워드` `경쟁 공백` `콘텐츠 방향` `검색 의도` `콘텐츠 전략` `상위 콘텐츠 패턴`. 추천 키워드 패널에는 **앰버 태그**가 붙음. 패널은 한번에 다 보여주지 않고 *0.4초 간격 stagger*.
- **카메라**: 3% push-in, 중앙 패널에 포커스
- **텍스트(UI)**: 위 6개 패널명
- **나레이션**: 1:33.0 *"발견된 기회는 / 다시 콘텐츠가 되고,"*
- **SFX**: 패널 등장 Low tick + 미세 Digital Ping, 핵심 패널에서 작은 Radar Scan
- **BGM**: 패드 + 피아노
- **전환**: 마우스 커서가 `CREATE CONTENT` 버튼으로 이동
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]`

#### C25 · 1:38.0–1:40.0 · CREATE CONTENT 클릭
- **화면**: 버튼 `CREATE CONTENT` 호버 → 클릭. 버튼 경계에서 **얇은 링 펄스**.
- **텍스트**: 버튼 `CREATE CONTENT`
- **나레이션**: (C24 나레이션 여운)
- **SFX**: **탐사 장비 작동음** — 잠금 해제 "thunk" + 짧은 상승 톤 (일반 UI 클릭음 금지)
- **BGM**: 펄스 +
- **전환**: 즉시 C26
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]`

#### C26 · 1:40.0–1:43.0 · 콘텐츠 생성
- **화면**: SEDNA가 분석 결과를 기반으로 **콘텐츠를 생성하는 장면**. 제목 → 소제목(H2) → 본문이 *자연스럽게 타이핑되듯* 흐르고, 이미지 슬롯이 채워진다. 생성 중 오른쪽 작은 패널에 사용된 근거(키워드/공백/의도)가 흐른다.
- **카메라**: 콘텐츠 영역 2% 줌인
- **나레이션**: 1:40.0 *"콘텐츠는 / 새로운 고객과 연결됩니다."*
- **SFX**: Data Processing 스트림, 작은 Digital Ping
- **BGM**: 스트링 스웰 정점 직전
- **전환**: 생성된 콘텐츠가 화면 뒤로 밀려나며 **지도 축소**(C27)
- **제작**: 🟦 `[REAL]` + 🟧 `[AE]`

---

### SCENE 08 — HORIZON (1:43–1:55)
**BGM M7 "HORIZON"** — 웅장한 앰비언트. 펄스 종료, 스트링+패드가 펼쳐진다. 1:54 이후 모든 악기 페이드, 드론만 남김.

#### C27 · 1:43.0–1:46.5 · 역방향 탐사 (지도 → 우주)
- **화면**: 경주 지도에서 **카메라가 뒤로 빠진다**. 경주 → 경상북도 → 대한민국 → 지구 → 우주. C11~C12의 역순을 *더 부드럽고 빠르게*. 핀들은 작은 점이 되어 사라진다. 경주의 앰버 포인트 하나만 마지막까지 남는다.
- **카메라**: 일정한 속도로 **long pull-back** (이징 0.22/0.0/0.0/1.0)
- **나레이션**: 없음 (BGM 중심)
- **SFX**: 역방향 Satellite Whoosh(저역), 대기 이탈 시 공기음 저하
- **BGM**: 스웰 정점
- **전환**: 연속
- **제작**: 🟦 `[REAL]` (지도/지구본 역재생 녹화) + 🟩 `[3D]`

#### C28 · 1:46.5–1:49.0 · 탐사선이 지구 앞을 지나간다
- **화면**: 우주에서 지구 전체를 바라보는 와이드샷. **NEW HORIZONS 탐사선**이 프레임 전경을 좌→우로 천천히 지나간다(실루엣+림라이트). 한반도는 지구 회전 방향으로 이동하며 뒤편으로 넘어가는 중이고, 경주 방향의 야간면에 **희미한 앰버 점 1개**가 남아 있다.
- **카메라**: 로우앵글 lock-off + 미세 드리프트
- **나레이션**: 없음 (정적)
- **SFX**: 스러스터 저주파 + 매우 작은 Satellite Signal
- **BGM**: 정점에서 한 박 쉼
- **전환**: 탐사선이 프레임 밖으로 나가며 화면 중앙에 로고 공간 확보
- **제작**: 🟪 `[AI]` 메인 + 🟩 `[3D]` 탐사선 합성

#### C29 · 1:49.0–1:51.5 · SEDNA 로고
- **화면**: 지구 위에 **SEDNA** 로고가 페이드인. 아래 작게 **`MARKET EXPLORATION SYSTEM`**. 로고 글자는 별빛이 모이는 방식(점 → 글자)으로 형성.
- **텍스트**: **`SEDNA`** / **`MARKET EXPLORATION SYSTEM`**
- **나레이션**: 없음
- **SFX**: Deep Cinematic Boom(약하게, 시그니처), 긴 리버브 테일
- **BGM**: 메인 테마 6음 모티프 피아노
- **전환**: 로고 유지 + 지구 미세 감속
- **제작**: 🟧 `[AE]`

#### C30 · 1:51.5–1:54.0 · 태그라인
- **화면**: 로고가 약간 위로 이동(또는 -20% 스케일)하고, 그 아래 **두 줄 태그라인**이 차례로 등장.
  `검색하지 마십시오.` (1:51.8) → `탐사하십시오.` (1:52.8, 더 밝게)
  영문: `DON'T SEARCH.` → `EXPLORE.`
- **나레이션**: 1:51.8 *"검색하지 마십시오."* (쉼 0.8s) *"탐사하십시오."* — **가장 낮고 차분한 톤**
- **SFX**: 마지막 단어에서 Sub Bass Hit 한 번
- **BGM**: 정점 → 모든 악기 해제, 패드만
- **전환**: 텍스트 유지 → 페이드
- **제작**: 🟧 `[AE]`

#### C31 · 1:54.0–1:55.0 (+3s 테일) · 엔드카드
- **화면**: 태그라인이 사라지고 **`SEDNA`** / 아래 `Powered by NEW HORIZONS ENGINE` (Mono, 불투명도 60%). 지구는 천천히 블랙으로 잠김.
- **나레이션**: 없음
- **SFX**: 드론 페이드아웃
- **BGM**: 웅장한 앰비언트 → 1:55부터 3초에 걸쳐 완전 암전·무음
- **전환**: **암전** (페이드 투 블랙 2초)
- **제작**: 🟧 `[AE]`

---

## 4. 전체 타임라인 요약표

| 컷 | TC | 길이 | 핵심 | 제작 |
|---|---|---|---|---|
| C01 | 0:00–0:03 | 3.0 | 암흑, 별 | 🟪/🟩 |
| C02 | 0:03–0:07 | 4.0 | 지구 림 | 🟪/🟩 |
| C03 | 0:07–0:12 | 5.0 | 지구 자전, THE UNKNOWN MARKET | 🟪/🟩/🟧 |
| C04 | 0:12–0:16.5 | 4.5 | 한국 접근, 도시 포인트 | 🟩/🟧 |
| C05 | 0:16.5–0:18.5 | 2.0 | 정적 | 🟩/🟧 |
| C06 | 0:18.5–0:25 | 6.5 | 질문, 탐사선, NEW HORIZONS ENGINE | 🟩/🟪/🟧 |
| C07 | 0:25–0:29 | 4.0 | 탐사선 → 지구 | 🟩/🟪/🟧 |
| C08 | 0:29–0:31 | 2.0 | 우주→UI 전환 | 🟧 |
| C09 | 0:31–0:36 | 5.0 | 검색창 경주/숙소 | 🟦/🟧 |
| C10 | 0:36–0:38 | 2.0 | MISSION START | 🟦/🟧 |
| C11 | 0:38–0:43 | 5.0 | 우주→한국 | 🟦/🟩 |
| C12 | 0:43–0:47 | 4.0 | 경북→경주 | 🟦/🟧 |
| C13 | 0:47–0:51 | 4.0 | 지도, 핀 01~10 | 🟦/🟧 |
| C14 | 0:51–0:55 | 4.0 | SCANNING MARKET | 🟦/🟧 |
| C15 | 0:55–0:59 | 4.0 | 엔진 가동 | 🟧/🟦 |
| C16 | 0:59–1:03 | 4.0 | TOP10·글자수·이미지 | 🟦/🟧 |
| C17 | 1:03–1:07 | 4.0 | 키워드·경쟁자·플레이스 | 🟦/🟧 |
| C18 | 1:07–1:12 | 5.0 | 검색의도·구조 → 별자리 | 🟦/🟧/🟩 |
| C19 | 1:12–1:17 | 5.0 | 시장 성단 | 🟩/🟧 |
| C20 | 1:17–1:21 | 4.0 | 공백을 향한 전진 | 🟩/🟧 |
| C21 | 1:21–1:24 | 3.0 | 정적→스캔→IMPACT | 🟧/🟩 |
| C22 | 1:24–1:30 | 6.0 | 롱테일 키워드 6개 | 🟧/🟩 |
| C23 | 1:30–1:33 | 3.0 | OPPORTUNITY FOUND, 새 별 | 🟪/🟩/🟧 |
| C24 | 1:33–1:38 | 5.0 | 결과 화면 | 🟦/🟧 |
| C25 | 1:38–1:40 | 2.0 | CREATE CONTENT | 🟦/🟧 |
| C26 | 1:40–1:43 | 3.0 | 콘텐츠 생성 | 🟦/🟧 |
| C27 | 1:43–1:46.5 | 3.5 | 지도→우주 | 🟦/🟩 |
| C28 | 1:46.5–1:49 | 2.5 | 탐사선 통과 | 🟪/🟩 |
| C29 | 1:49–1:51.5 | 2.5 | SEDNA 로고 | 🟧 |
| C30 | 1:51.5–1:54 | 2.5 | 태그라인 | 🟧 |
| C31 | 1:54–1:55 | 1.0 | 엔드카드 → 암전 | 🟧 |

---

## 5. 제작 구분별 체크리스트

### 5-1. 🟦 실제 SEDNA 화면 촬영이 필요한 구간
| # | 화면 | 사용 컷 | 녹화 사양 |
|---|---|---|---|
| 1 | 검색창 (지역=경주 / 업종=숙소, 타이핑) | C09, C10 | 4K 60fps, 커서 경로 사전 스크립트, 타이핑 1.2배속 |
| 2 | 3D 지구본 (회전) | C11 | Three.js 카메라 경로를 고정 스크립트로 |
| 3 | 지역 줌인 (한국→경북→경주) | C11, C12 | 카메라 패스 기록, ease 5초 |
| 4 | 지도 (경주) | C13 | 지도 타일은 저채도·다크 테마 |
| 5 | 분석 핀 01~10 | C13, C14 | 핀 생성 간격 0.25초 |
| 6 | TOP10 분석 | C16 | 글자수/이미지 수 막대 포함 |
| 7 | 경쟁 콘텐츠 | C17 | 블로그 제목은 **가상/익명화 처리 필수** (실제 블로그명·작성자 노출 금지) |
| 8 | 키워드 분석 | C17 | 빈도 차트 |
| 9 | MARKET GAP | C21~C22 | 실제 화면이 있으면 보조로만 사용 (메인은 3D/AE 연출) |
| 10 | 추천 키워드 / 결과 패널 | C24 | 6개 패널 |
| 11 | CREATE CONTENT 클릭 | C25 | 호버→클릭 |
| 12 | 콘텐츠 생성 | C26 | 타이핑 생성 과정 |

**촬영 팁**
- 녹화용 데이터는 **시드 고정**: 경주/숙소 결과 스냅샷을 미리 저장하고 네트워크 지연 없이 재생
- 모든 UI 컷은 **클린 플레이트(개인정보·실제 계정명 제거)**
- UI는 **다크 모드 + 불필요한 사이드 메뉴 숨김**. 촬영 전 UI 스케일 150~200% 권장(영상에서 글자 가독성)
- 화면 전체를 보여주기보다 **패널 단위로 크롭**하여 사용 (요청서의 "UI 전체 노출 금지" 준수)
- 실제 네이버 블로그/플레이스 데이터가 화면에 나올 경우 **제3자 콘텐츠의 공개 사용 권리** 검토 필요 → 샘플 데이터로 대체 권장

### 5-2. 🟪 AI 영상 생성이 필요한 구간
C01, C02, C03(보조), C06(탐사선 히어로), C07(보조), C23(별 탄생), C28(탐사선 통과) — §7에 프롬프트
※ AI 모델은 **지도 텍스트·라벨·한글 글자를 정확히 생성하지 못합니다.** 텍스트는 전부 AE에서 오버레이.
※ 지구·한반도 지형의 정확성이 필요한 컷(C04, C11, C12)은 AI가 아닌 3D/실제 UI 사용 권장.

### 5-3. 🟧 After Effects 제작 구간
C03 타이틀, C04 라벨/라인, C06 타이틀, C07–C08 전환, C09–C10 글로우/링 펄스, C12/C13 리플, C14 스캔 링, C15 엔진 코어, C16 패럴랙스, C18 분해 전환, C19–C22 스캔 라인·AMBER 하이라이트·키워드, C23 타이틀, C24–C26 UI 합성, C29–C31 로고/태그라인/엔드카드

**AE 컴포지션 구조**
```
00_MASTER (3840x2160, 24fps)
 ├─ 01_SPACE_PLATES      (AI/3D 렌더 플레이트)
 ├─ 02_UI_CAPTURES       (실제 SEDNA 녹화)
 ├─ 03_TYPE              (타이틀, 라벨, 키워드)
 ├─ 04_DATA_FX           (스캔 라인, 링, 리플, 점 구름)
 ├─ 05_TRANSITIONS       (C08, C12→C13, C18→C19)
 ├─ 06_COLOR             (Adjustment + LUT + Grain)
 └─ 07_END               (C29~C31)
```
- 공통 룩: **필름 그레인 2~3%**, 비네트 -10%, 블룸 약하게(Glow threshold 80%, radius 30), 색수차 0.2px(거의 안 보이게)
- 렌즈플레어 금지, 글리치 금지

### 5-4. 🟩 Blender / Three.js 제작 구간
| 구간 | 권장 툴 | 설명 |
|---|---|---|
| 지구(C01–C07) | **Blender** | 8K 지구 텍스처(블루마블 계열, 사용 조건 확인), 야간 도시광, 대기 셰이더(Fresnel), 구름 레이어 분리 |
| 탐사선(C06–C07, C28) | **Blender** | 오리지널 딥스페이스 프로브, 골드 포일 PBR, 림라이트 |
| 한반도/행정경계 라인(C04) | **Blender** 또는 AE | GeoJSON → Curve → 1px 라인 렌더 |
| SEDNA 3D 지구본(C11–C12, C27) | **Three.js (실제 프로그램)** | 실제 기능이므로 화면 녹화, 카메라 패스를 JSON으로 저장해 재생 |
| 시장 성단/점 구름(C18–C22) | **Three.js / Blender Geometry Nodes** | 경주 숙소 키워드·블로그 글을 실제 데이터로 점 생성 → 공백 위치는 *클러스터링 결과의 빈 공간*을 사용 |
| 새 별(C23) | **Blender** | 앰버 포인트 라이트 + 회절 링 |

**Three.js 지구본 카메라 패스 (참고 스펙)**
```js
// 예: 키프레임(고도km, 위도, 경도, 피치°)
const path = [
  { t: 0.0, alt: 35786, lat: 20, lng: 120, pitch: 0 },
  { t: 2.5, alt:  4000, lat: 36, lng: 128, pitch: 45 },
  { t: 4.5, alt:   620, lat: 36.0, lng: 129.2, pitch: 60 },  // 경북
  { t: 5.0, alt:   120, lat: 35.84, lng: 129.21, pitch: 70 } // 경주
];
// easing: easeInOutCubic, 지구 자전 없음(촬영 중 고정)
```

---

## 6. 사운드 디자인 & 음악

### 6-1. BGM 큐시트
| 큐 | 구간 | 성격 | BPM | 핵심 |
|---|---|---|---|---|
| M1 VOID | 0:00–0:25 | 우주 다큐 앰비언트 | 무박 | D 마이너 드론, 글래스 패드, 서브 럼블 |
| M2 SIGNAL | 0:25–0:38 | 펄스 진입 | 72 | 서브 베이스 플럭, 얇은 아르페지오 |
| M3 DESCENT | 0:38–0:55 | 탐사 시작, 리듬 증가 | 90 | 하이햇 진입, 베이스 펄스 |
| M4 ANALYSIS | 0:55–1:12 | 밀도 증가 | 96 | 미세 퍼커션 클릭, 펄스 상승 |
| M5 THE VOID | 1:12–1:24 | 음악 낮춤 → 임팩트 | — | 드론만, 1:21 정적, **1:23.0 임팩트** |
| M6 FOUND | 1:24–1:43 | 상승 | 84 | 앰버 패드, 피아노 모티프, 스트링 스웰 |
| M7 HORIZON | 1:43–1:58 | 웅장한 앰비언트 | — | 스트링+패드 펼침 → 드론 → 암전 |

**피아노 모티프 (6음 · 제안)**: D4–F4–A4–C5–A4–F4 (롱테일 키워드 6개와 동기). 로고에서 같은 모티프 재등장.

### 6-2. 음악 검색 키워드 (라이선스 음원 탐색용)
`Cinematic Space Documentary` · `NASA Documentary Music` · `Deep Space Ambient` · `Technology Documentary` · `Future Exploration` · `Space Discovery` · `Cinematic Drone Sub Bass Build`
※ 상업 광고 사용 라이선스(Sync + Master, 온라인/TV 포함) 확인 필수. 창작 음악을 의뢰한다면 위 큐시트를 그대로 작곡 브리프로 사용 가능.

### 6-3. 효과음 라이브러리 (검색어 + 사용처)
| SFX | 용도 |
|---|---|
| Deep Space Rumble | C01~C06 전반 저역 |
| Satellite Signal | 원거리 신호 핑 (C01, C06, C19…) |
| Radar Scan | 스캔 라인/링 (C14, C21) |
| Data Processing | 엔진 분석 (C15~C18, C26) |
| Digital Ping | 핀, 키워드, 포인트 (음정 체계 유지: D, F, A 계열) |
| Low Frequency Impact | MISSION START, GAP |
| Satellite Whoosh | 카메라 이동 (C04, C07, C11, C27) |
| Sub Bass Hit | 텍스트 임팩트 (C08, C21, C30) |
| Deep Cinematic Boom | **MARKET GAP DETECTED(C21)**, 로고(C29) |

**믹싱 룰**: 나레이션 -14 LUFS 기준, 음악은 나레이션 구간에서 -8dB 덕킹, SFX는 대사 주파수(1–4kHz) 회피. **클릭음은 일반 UI 클릭 대신 "탐사 장비 잠금 해제/작동음"** 으로 디자인.

---

## 7. 컷별 AI 영상 생성 프롬프트 (EN)

### 7-0. 공통 스타일 블록 (모든 프롬프트 앞에 붙임)
```
STYLE BLOCK:
Cinematic space documentary footage, shot on large-format IMAX-style camera, 2.39:1 framing, restrained and minimal, deep blue and black color palette, subtle film grain, realistic physically based lighting, no text, no logos, no watermark, no on-screen graphics, slow deliberate camera motion, premium brand film quality in the spirit of a NASA exploration documentary.
```

### 7-0b. 공통 네거티브 프롬프트
```
NEGATIVE: text, letters, watermark, logo, NASA logo, UI, HUD overlays, neon colors, cyberpunk, glitch, lens flare, excessive bloom, cartoon, stylized, sci-fi movie spaceship, Star Wars, fast camera movement, shaky camera, jump cuts, humans, faces, astronaut, low resolution, warped planet, visible seams, extra moons
```

### C01 — Stars in darkness (5s, 2160p)
```
[STYLE BLOCK] Complete darkness. Stars slowly fade into view one by one across a pure black sky until a rich, deep star field emerges, with varied star brightness and a faint cool-blue Milky Way haze at the bottom edge. Camera is almost static with an extremely slow forward drift. Very subtle twinkling, no planet yet. Contemplative, silent, vast.
Camera: slow push-in, 0.5% per second. Duration 5s. Aspect 21:9.
```

### C02 — Earth limb rising (6s)
```
[STYLE BLOCK] Above a star field, the curved edge of Earth slowly appears at the bottom of frame, lit by a low sun from the upper left beyond the frame. A thin luminous cyan-blue atmospheric rim glows along the limb; city lights on the night side are barely visible. Camera performs a slow dolly-in with a very slight upward tilt. Everything moves at a deliberate, weightful, documentary pace. High realism, scientifically plausible Earth from low orbit.
Camera: slow dolly-in + 2° tilt up. Duration 6s.
```

### C03 — Rotating Earth hero (6s)
```
[STYLE BLOCK] A photoreal Earth seen from space in a wide shot, slowly rotating, occupying the center of frame against a black star field. Deep blue oceans, thin realistic cloud layers, a soft terminator line, faint golden city lights on the night side. Extremely slow camera dolly towards the planet, slowing down at the end. Calm, majestic, no lens flare, no extra glow beyond a subtle atmospheric rim.
Camera: slow dolly-in decelerating to near stop. Duration 6s.
```

### C04 — Approaching East Asia at night (plate, use with 3D overlay) (6s)
```
[STYLE BLOCK] Orbital view descending toward East Asia on the night side of Earth. The Korean peninsula is softly visible by scattered warm-white city lights along the coasts, with sparse lights across mountains. Thin atmospheric haze, stars at the top of the frame. Camera descends slowly and tilts from a high angle toward a more oblique angle. No labels, no lines, no text. Realistic geography, calm.
Camera: orbital descent with gentle tilt, 6s.
```
> ※ 지명·라인·포인트는 AE에서 추가. 지형 정확성이 중요하면 이 컷은 AI 대신 Blender 플레이트 사용.

### C06 — Probe hero reveal (6s)
```
[STYLE BLOCK] A small original deep-space exploration probe appears at the center of frame above Earth's limb, rear three-quarter view from slightly low angle. The probe has a gold-foil wrapped body, a large white parabolic high-gain antenna dish, a long boom and a small instrument deck. A faint cool-blue ion thruster glow. Sunlight rim-lights the gold foil with soft reflections of the Earth's blue glow. Extremely slow push-in, the probe drifts weightlessly and steadily. Understated, realistic, no NASA markings, no text.
Camera: slow push-in, slight parallax against star background. Duration 6s.
```

### C07 — Probe travels toward Earth (5s)
```
[STYLE BLOCK] Tracking shot behind and slightly above a small original gold-foil deep-space probe as it glides steadily toward a huge Earth filling the lower half of the frame. Blue engine glow at the back of the probe, reflected earthlight on the gold foil, tiny micro-rotations in attitude control. Earth's atmosphere glows as a thin blue line. Smooth, cinematic, slow.
Camera: smooth tracking behind probe with very slight roll (+0.5°). Duration 5s.
```

### C08 — Atmosphere entry transition plate (3s)
```
[STYLE BLOCK] Camera slowly pushes into Earth's upper atmosphere, from black space into soft deep-blue haze. The frame gradually fills with a smooth gradient from #0B2A4A to #07111F, no clouds detail, no bright flash, no lens flare. Ends on a nearly flat dark-blue gradient suitable for a clean dissolve into a user interface.
Camera: forward push, motion blur increasing then settling. Duration 3s.
```

### C19 — Star-field market nebula (plate for the point-cloud scene) (6s)
```
[STYLE BLOCK] Inside a vast dark nebula, thousands of small cool-blue points of light form several dense clusters like constellations, separated by a conspicuously dark empty region in the middle. The clusters subtly avoid the empty area. Depth of field shallow, tiny particles float. Camera drifts forward slowly between the clusters. Mysterious, silent, scientific. No text, no lines, no connecting wires.
Camera: slow forward drift with slight parallax. Duration 6s.
```

### C20 — The void (5s)
```
[STYLE BLOCK] Slow push-in toward a dark gap among blue star clusters. The empty region is not pure black but holds an extremely faint warm amber shimmer, barely perceptible. Surrounding star points are sharp, cold blue. The gap feels like unexplored territory. Camera speed gradually decreases.
Camera: slow push-in decelerating, 5s.
```

### C23 — A new star is born (5s)
```
[STYLE BLOCK] In the dark empty region between blue star clusters, a single warm amber point of light gradually condenses and brightens into a new star. Surrounding blue stars pick up a subtle warm rim from its light. A soft circular diffraction ring expands once and fades. No flares, no explosion, just a calm, dignified sunrise-like birth of light. Camera pushes in gently toward the star.
Camera: slow push-in. Duration 5s.
```

### C27 — Pull-back from atmosphere to space (plate) (5s)
```
[STYLE BLOCK] Reverse orbital ascent: camera rises smoothly from a thin cloud layer over East Asia up through the atmosphere into space, revealing the curvature of Earth and then the whole planet against stars. Constant steady speed with a long deceleration. Calm, majestic.
Camera: steady pull-back with soft ease-out. Duration 5s.
```

### C28 — Probe passes in front of Earth (4s)
```
[STYLE BLOCK] Wide shot of a fully visible Earth in space, slightly low angle. In the foreground, a small original deep-space probe crosses the frame slowly from left to right as a rim-lit silhouette with gold-foil highlights, passing in front of the planet. The planet's night side shows faint city lights; one tiny warm amber point glows on the night side of the Korean peninsula. Camera locked off with very subtle drift.
Camera: lock-off, slight drift. Duration 4s.
```

### C29/C31 — Logo background plate (4s)
```
[STYLE BLOCK] Earth in deep space slowly rotating, framed in the lower half of the frame leaving a large clean dark space at the top and center for a logo. Deep blue atmosphere, faint stars, no text, no graphic elements. Extremely slow push-in then a soft fade to black at the end.
Camera: extremely slow push-in. Duration 4s. Ends with fade to black.
```

**툴별 권장 세팅**
| 모델 | 권장 |
|---|---|
| Veo | 긴 호흡·카메라 지시에 강함 → C01–C03, C23, C28 |
| Kling | 탐사선 모션/전경 합성 → C06, C07 |
| Runway | 이미지→비디오(탐사선 스틸 기반 일관성) → C06/C07/C28 |
| Sora | 질감·빛 표현 → C19, C20, C23 |
**일관성 팁**: 탐사선은 Midjourney/이미지 모델로 *스틸 1장을 먼저 확정*하고, 모든 탐사선 컷을 이미지→비디오(I2V)로 생성. 프롬프트에 동일한 탐사선 묘사 문장을 고정 사용.

---

## 8. 브랜드 : UI 비율 점검 (목표 50:50)

| 구분 | 구간 | 초 |
|---|---|---|
| 브랜드 필름(우주·3D·AI·타이포) | C01–C08 (29s) · C19–C23 (약 23s) · C27–C31 (12s) | ≈ 64s |
| 실제 UI | C09–C18 (약 35s) · C24–C26 (11s) | ≈ 46s |
| 합계 | | 110s (+ C21/22 등 합성 구간 겹침) |

→ 브랜드 ≈ **55–58%** / UI ≈ **40–45%**. 요청(약 50:50)에 근접하되, UI를 더 줄이려면 **C16–C17 각각 0.5초 단축** 및 C24를 패널 일부만 노출. UI를 더 늘리려면 C09 타이핑 구간을 1초 연장. 또한 C16~C18의 UI는 3D 공간에 띄운 패럴랙스/분해 전환을 적용해 "UI를 보여주는" 시간이 아니라 "탐사의 일부"로 읽히게 한다.

---

## 9. 튜닝 포인트 (편집자용)

1. **나레이션 속도**: 한국어 기준 약 4.0–4.5 음절/초로 설계. 녹음 후 전체가 1:55를 넘으면 S05의 SFX 간격을 줄이지 말고, **S01–S02 쉼 길이**를 먼저 조정.
2. **임팩트 포인트 1:23.0**: 이 프레임에 **나레이션·스캔음·텍스트·음악 임팩트가 동시에 정렬**되어야 한다. 이 지점을 기준으로 역산해 편집 가능.
3. **AMBER 사용 제한**: C21 이전에는 앰버가 **한 번도 나오면 안 된다**. (C20의 미세한 잔광은 예외이며, 육안으로는 거의 보이지 않는 수준)
4. **텍스트 총량**: 영상 전체에서 동시에 화면에 있는 텍스트 블록은 **최대 3개**.
5. **레퍼런스 영상 톤 맞추기**: 원본 시청 후 (a) 첫 12초 호흡 (b) 자막 크기 (c) BGM 텐션 곡선만 참고, 샷/대사는 복제 금지.

---

## 10. 전체 나레이션 (별도 정리)

**[SCENE 01]**
우리가 매일 검색하는 인터넷에는
수없이 많은 정보가 존재합니다.
검색량.
콘텐츠.
경쟁자.
그리고 아직 아무도 발견하지 못한 기회.

**[SCENE 02]**
하지만 우리는
그 대부분을 발견하지 못한 채 지나칩니다.

*(정적 2초)*

그렇다면,
이 거대한 데이터 속에서
우리가 원하는 시장만
탐사할 수 있다면 어떨까요?

**[SCENE 03]**
우리는 이 탐사를 위해
하나의 시스템을 만들었습니다.

*(검색창 구간 — 무음)*

SEDNA.

**[SCENE 04]**
SEDNA는 지역을 탐색하고
시장을 스캔합니다.
검색 결과를 보는 것이 아니라
시장이 어떻게 움직이고 있는지를
추적합니다.

**[SCENE 05]**
SEDNA의 뉴호라이즌스 엔진은
수많은 데이터를 하나씩 분석합니다.
어떤 콘텐츠가 상위에 있는지.
경쟁자는 무엇을 이야기하고 있는지.
사람들은 무엇을 찾고 있는지.

**[SCENE 06]**
하지만 SEDNA가 찾는 것은
이미 존재하는 데이터만이 아닙니다.
경쟁자가 놓친 영역.
아직 충분히 다뤄지지 않은 검색어.
바로,

*(정적 1초 — MARKET GAP DETECTED)*

시장에 남아 있는
빈 공간입니다.

**[SCENE 07]**
발견된 기회는
다시 콘텐츠가 되고,
콘텐츠는
새로운 고객과 연결됩니다.

**[SCENE 08]**
검색하지 마십시오.
탐사하십시오.

*(EN 화면 카피: DON'T SEARCH. EXPLORE. / SEDNA — Powered by NEW HORIZONS ENGINE)*

**성우 디렉션**: 중저음, 과장 없는 다큐 톤. 감정은 "놀람"이 아니라 "경외". 문장 끝을 올리지 말고 **내려서 마무리**. "SEDNA."와 "탐사하십시오."는 이 영상에서 가장 낮고 조용하게.

---

## 11. 영어 화면 카피 (온스크린 텍스트 총정리)

| TC | 텍스트 |
|---|---|
| 0:09 | THE UNKNOWN MARKET |
| 0:12 | SEOUL · BUSAN · DAEGU · GYEONGJU · POHANG (라벨) |
| 0:23 | NEW HORIZONS |
| 0:24 | NEW HORIZONS ENGINE |
| 0:36 | MISSION START |
| 0:38 | ORBIT / ALT (Mono 장식) |
| 0:43 | GYEONGBUK → GYEONGJU |
| 0:51 | SCANNING MARKET |
| 0:55 | ANALYZING… / SCANNING… / PROCESSING… |
| 0:55–1:12 | TOP CONTENT · TOP 10 · KEYWORD · COMPETITOR · PLACE · SEARCH INTENT · CONTENT LENGTH · IMAGE · BLOG · LOCAL SEARCH · KEYWORD FREQUENCY · CONTENT STRUCTURE |
| 1:23 | MARKET GAP DETECTED |
| 1:24 | LONG-TAIL KEYWORD |
| 1:30 | OPPORTUNITY FOUND |
| 1:38 | CREATE CONTENT |
| 1:49 | SEDNA / MARKET EXPLORATION SYSTEM |
| 1:51 | DON'T SEARCH. / EXPLORE. |
| 1:54 | SEDNA — Powered by NEW HORIZONS ENGINE |

---

## 12. 제작 순서 권장 (파이프라인)

1. **보이스 가이드 녹음(가녹음)** → 타이밍 확정 (애니매틱의 기준)
2. **SEDNA UI 녹화 세트** (§5-1, 카메라 패스 JSON 포함)
3. **Blender 지구/탐사선 렌더** + **AI 플레이트 생성**
4. **AE 합성**: 플레이트 → 전환 → UI → 타이포
5. **사운드 디자인 + 작곡/라이선스 BGM**
6. **C21(1:23.0) 기준 싱크 체크**
7. **컬러 마스터 + 그레인 + 마스터링(-14 LUFS)**
8. **버전 제작**: 1:55 마스터 / 30초 컷다운(C01→C06→C21→C22→C30) / 세로(9:16) 버전은 UI 중심 재구성

---

## 13. 최종 체크: "기능 소개 영상처럼 보이지 않는가?"

- [ ] 첫 25초 동안 **SEDNA라는 이름이 나오지 않는다** (나오는 건 질문과 우주뿐)
- [ ] UI는 **결코 전체 화면으로 오래 머물지 않고**, 항상 카메라 이동 안에 있다
- [ ] 기능 나열은 S05 **4초씩 3단**으로만 (리스트 나열 금지)
- [ ] 가장 길고 강한 장면은 **MARKET GAP** (C19–C22)
- [ ] 마지막에 남는 단어는 **탐사하십시오 / EXPLORE.**
- [ ] 관객의 요약: *"이건 검색 프로그램이 아니라 시장을 탐사하는 시스템이구나."*
