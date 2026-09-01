# 🎨 Chaereve ColorLab

<p align="center">
  <a href="https://github.com/chaereve/chaereve-colorlab/releases"><img alt="다운로드" src="https://img.shields.io/badge/%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C-2ea043?style=for-the-badge"></a>
</p>

<p align="center">
  <a href="README.md"><img alt="English" src="https://img.shields.io/badge/English-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.vi.md"><img alt="Tiếng Việt" src="https://img.shields.io/badge/Ti%E1%BA%BFng%20Vi%E1%BB%87t-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.zh.md"><img alt="中文" src="https://img.shields.io/badge/%E4%B8%AD%E6%96%87-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ko.md"><img alt="한국어" src="https://img.shields.io/badge/%ED%95%9C%EA%B5%AD%EC%96%B4-22d3ee?style=for-the-badge"></a>&nbsp;
  <a href="README.ja.md"><img alt="日本語" src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.es.md"><img alt="Español" src="https://img.shields.io/badge/Espa%C3%B1ol-1a3fd6?style=for-the-badge"></a>
</p>

Photoshop(`.aco`) 색상 팔레트를 **보고, 섞고, 내보내는** 도구로, **브라우저 안에서** 완전히 동작합니다. 설치 불필요, 가입 불필요, 데이터 업로드 없음.

> 모든 데이터는 기기에서 **100% 로컬로** 처리됩니다.

**🌐 다국어 UI (6개 언어):** Tiếng Việt, English, 中文 (简体), 한국어, 日本語, Español — **⚙️ 설정**에서 전환.

---

## ✨ 기능

### 📁 ACO 보기
- `.aco` 파일을 드래그 앤 드롭(또는 클릭)하여 엽니다.
- **ACO v1 & v2** 지원, **색상 이름**과 RGB / HSB / CMYK / Lab / Grayscale 색공간을 읽습니다.
- 각 색상은 **색인 번호**, 이름, HEX, RGB 및 원래 색공간을 표시합니다.
- 이름/HEX/RGB로 **검색**하고 색상, 밝기, 채도, 이름으로 **정렬**합니다.
- **고급 검색** — `hue:0-60`, `sat:>50`, `light:40-80` 범위로 필터링하거나 `similar:#FF0000`으로 비슷한 색을 찾습니다.

### ✏️ 팔레트 편집 (제자리 편집)
- 색상 **이름 바꾸기**(✏️), **삭제**(🗑), **추가** 후 **.aco로 다시 저장**합니다.
- 완전한 **실행 취소 / 다시 실행** (최대 60단계).
- 색상 칩을 **우클릭**하여 빠른 메뉴(복사 / 상세 / 이름 바꾸기 / 내보내기 / 삭제)를 엽니다.

### 📋 복사
- 색상 칩을 클릭하면 코드(**HEX / RGB / HSL** — 선택 가능)를 복사합니다.
- **전체 복사**: HEX 목록, CSS 변수, SCSS, JSON, RGB, **Tailwind config**, **Styled Components**.

### 🎨 색상 혼합 (독립 사용 — ACO 불필요)
- **색상 선택기**로 색을 추가하거나 이 탭에서 바로 **ACO 파일을 엽니다**.
- 선택 그리드로 **섞고 싶지 않은 색을 한 번의 클릭으로 제외**합니다.
- 파일을 다시 올리지 않고 **선택을 재조정**합니다.
- 비율은 색상 수에 따라 **자동 균등 분배**; 슬라이더로 개별 조정.
- **혼합 기록**이 자동 저장되며 클릭하면 다시 복사됩니다.

### 🎲 랜덤 색상 (멤버별)
- 각 "멤버"에 대해 1–100개의 랜덤 색상을 생성합니다. 완전 랜덤 또는 선택한 색상 계열(빨강 / 주황 / 노랑 / 초록 / 시안 / 파랑 / 보라 / 분홍) 내에서, 중복 없음 모드 선택 가능.

### 🛠 디자인 도구
두 탭으로 분리 — **🧩 만들기**와 **🔍 분석**:
- **팔레트 생성기** — 보색 / 유사 / 삼각 / 분할 / 사각.
- **그라디언트 생성기** — 선형 / 방사형 / **원뿔** CSS 그라디언트, 복사 기능.
- **이미지 → 팔레트 / 스포이드** — 이미지를 클릭해 색을 고르고, 주 색상을 추출해 **바로 .aco로 내보냅니다**.
- **프리셋 & 템플릿** — 내장 Material Design, Tailwind, Brand Colors, Pastel, Earth Tones 팔레트.
- **대비 검사기** — AA/AAA 배지가 있는 WCAG 대비율.
- **접근성 감사** — 흰색/검정 텍스트에 대해 AA를 통과하는 팔레트 비율.
- **팔레트 통계** — 평균 채도/밝기와 색상 분포 차트.
- **색맹 미리보기** — 적색맹 / 녹색맹 / 청색맹 / 회색조.
- **색상 상세 패널** — HEX / RGB / HSL / HSV / CMYK / Lab, 휘도, 대비.
- **중복 감지기**와 **비슷한 색 찾기**.

### 📦 일괄 처리
- **여러 .aco 파일**을 한 번에 열어 하나의 팔레트로 **병합**(선택적 중복 제거)하거나 **병합된 .aco 내보내기**.

### 🔗 팔레트 공유
- 현재 팔레트를 인코딩한 **공유 링크**(`?palette=...`)를 생성합니다 — 링크를 여는 누구나 같은 색을 볼 수 있고 서버가 필요 없습니다.

### 📐 그라디언트 (.grd)
- Photoshop **그라디언트 파일**(`.grd`, **v3 & v5**) — 솔리드 및 노이즈 그라디언트를 엽니다.
- 각 그라디언트를 **미리보기**한 후 색상 정지점, 투명도 정지점, 중간점, 매끄러움, 노이즈 매개변수(시드, 거칠기, 최소/최대)를 **편집**합니다.
- 그라디언트와 정지점을 **추가 / 제거**하고 **`.grd`로 다시 저장**합니다.
- 그라디언트를 **CSS `linear-gradient`** 또는 **SVG**로 내보내고 색상을 **`.aco`로 추출**하거나 뷰어로 바로 보냅니다.

### ⬇ 내보내기
- 레이아웃, 크기, 라벨, 배경(투명 포함) 옵션이 있는 **PNG / SVG / CSS / JSON / TXT**.
- 선택한 색상의 **ACO 내보내기** (v2, 색상 이름 포함).

### 🌙 UI — 글래스모피즘
- **글래스모피즘** 디자인: 반투명 유리 패널, 부드러운 블러, 은은한 빛 — macOS/iOS처럼 세련됨.
- **다크 / 라이트 / 자동** 테마(기본적으로 시스템 따름).
- **6개 언어**: Tiếng Việt, English, 中文 (简体), 한국어, 日本語, Español — **⚙️ 설정**에서 전환 가능.
- 부드러운 애니메이션과 모바일 우선 레이아웃(하단 내비게이션, 바텀시트, 큰 터치 타깃).

### ⚙️ 설정
- **화면** — 라이트, 다크 또는 자동 테마.
- **강조 색상** — 전체 UI(로고, 탭, 버튼, 글로우)를 다시 칠합니다.
- **언어**와 **글자 크기** (작게 / 중간 / 크게).
- **사운드 효과** — 클릭, 복사, 알림 시 은은한 소리(켜기/끄기).
- **모션 효과** 켜기/끄기, **저장된 데이터 지우기**, **정보** 상자.

### 📲 앱으로 설치 (PWA)
- **데스크톱(Windows/macOS/Linux)** 및 **모바일(Android/iOS)**에 설치 가능.
- 자체 아이콘, 독립 창으로 열리고 **오프라인**으로 작동합니다.

### 🖥 데스크톱 버전 (Windows)
- Electron으로 **네이티브 Windows 데스크톱 앱**으로 패키징 — `electron-app/` 폴더 참조.
- **Windows** 설치 프로그램 빌드: `.exe` (설치 프로그램 + 포터블).
- 앱 로고는 현대 앱처럼 **둥근 모서리**로 처리됩니다.

---

## 🚀 사용법

### 데스크톱 / 모바일에서
아무 브라우저에서 `index.html`을 열거나(더블클릭), 배포된 URL을 방문하세요.

### 빠른 흐름
1. **📁 ACO 보기** 탭 열기 → `.aco` 파일 드래그 앤 드롭.
2. 색을 클릭해 복사하거나 여러 색을 선택해 내보냅니다.
3. **🎨 색상 혼합** 탭 열기 → 색 추가 → 혼합 결과 즉시 확인.
4. **⬇ 이미지 & 데이터 내보내기**를 클릭해 팔레트를 다운로드.
5. **📐 그라디언트** 탭 열기 → `.grd` 파일을 넣어 Photoshop 그라디언트 보기/편집.
6. **⚙️ 설정**을 열어 테마, 강조 색상, 언어, 글자 크기를 전환.

---

## 🌐 언어 (6개)

**⚙️ 설정**(우측 상단 톱니 버튼)을 열고 **언어** 메뉴에서 선택: Tiếng Việt, English, 中文 (简体), 한국어, 日本語, Español. 전체 인터페이스가 즉시 전환되고 선택 사항이 유지됩니다.

**이 저장소의 README와 사용자 가이드는 6개 언어로 제공됩니다:**

| 언어 | README | 사용자 가이드 |
|------|--------|---------------|
| 🇬🇧 English | [README.md](README.md) | [USER_GUIDE.md](USER_GUIDE.md) |
| 🇻🇳 Tiếng Việt | [README.vi.md](README.vi.md) | [USER_GUIDE.vi.md](USER_GUIDE.vi.md) |
| 🇨🇳 中文 (简体) | [README.zh.md](README.zh.md) | [USER_GUIDE.zh.md](USER_GUIDE.zh.md) |
| 🇰🇷 한국어 | [README.ko.md](README.ko.md) | [USER_GUIDE.ko.md](USER_GUIDE.ko.md) |
| 🇯🇵 日本語 | [README.ja.md](README.ja.md) | [USER_GUIDE.ja.md](USER_GUIDE.ja.md) |
| 🇪🇸 Español | [README.es.md](README.es.md) | [USER_GUIDE.es.md](USER_GUIDE.es.md) |

---

## 📲 앱으로 설치 (PWA)

앱이 배포되면(HTTPS) 실제 앱으로 설치할 수 있습니다:

| 플랫폼 | 방법 |
|--------|------|
| **데스크톱** (Chrome/Edge) | URL 열기 → **📲** 버튼 또는 주소창 설치 아이콘 → **설치** |
| **Android** (Chrome) | URL 열기 → **⋮** 메뉴 → **홈 화면에 추가** |
| **iPhone/iPad** (Safari) | URL 열기 → **공유** 버튼 → **홈 화면에 추가** |

> **중요:** PWA는 **HTTPS**로 제공되어야 합니다(GitHub Pages, Netlify, Vercel 모두 지원). `file://`을 직접 열면 설치할 수 없습니다.

---

## ❓ FAQ

**내 데이터가 어딘가에 업로드되나요?**
아니요. 모든 것이 브라우저에서 실행되며 네트워크로 아무것도 전송되지 않습니다.

**파일을 열었는데 색상이 안 보여요?**
유효한 `.aco` 파일인지 확인하세요. 일부 소프트웨어는 비표준 구조로 ACO를 내보냅니다.

**색상 혼합은 어떻게 작동하나요?**
앱이 비율(가중 평균)로 색상을 섞습니다 — 물감을 섞는 것처럼요. 슬라이더를 드래그해 색을 더 "무겁게" 만듭니다.

**파일의 일부 색만 섞으려면?**
**색상 혼합** 탭에서 ACO를 열고 → 원치 않는 색을 클릭해 해제 → **혼합에 색 추가** 클릭.

---

## 📚 가이드

사용자 가이드 (6개 언어):
- 🇬🇧 [USER_GUIDE.md](USER_GUIDE.md) · 🇻🇳 [USER_GUIDE.vi.md](USER_GUIDE.vi.md) · 🇨🇳 [USER_GUIDE.zh.md](USER_GUIDE.zh.md) · 🇰🇷 [USER_GUIDE.ko.md](USER_GUIDE.ko.md) · 🇯🇵 [USER_GUIDE.ja.md](USER_GUIDE.ja.md) · 🇪🇸 [USER_GUIDE.es.md](USER_GUIDE.es.md)

---

## 📄 라이선스

개인 및 상업적 용도로 자유롭게 사용 가능.
