# Yomitan 한국어 사전 모음

[English](#english)

웹페이지의 외국어 단어에 마우스를 올리면 **한국어 뜻**이 바로 뜨게 해 주는 사전들입니다.
무료 브라우저 확장 [Yomitan](https://yomitan.wiki/)에 넣어서 씁니다.

| 사전 | 방향 | 수록 | 받기 |
|---|---|---|---|
| [JMdict-ko](https://github.com/kongchu2/jmdict-ko) | 일본어 → 한국어 | 빈도 상위 50,049개 항목 + 한자 훈음 | [jmdict-ko.zip](https://github.com/kongchu2/jmdict-ko/releases/latest/download/jmdict-ko.zip) · [kanjidic-ko.zip](https://github.com/kongchu2/jmdict-ko/releases/latest/download/kanjidic-ko.zip) |
| [Wiktionary-en-ko](https://github.com/kongchu2/wiktionary-en-ko) | 영어 → 한국어 | 107,812개 항목 (상위 5만 단어, 구동사, 숙어) | [wiktionary-en-ko.zip](https://github.com/kongchu2/wiktionary-en-ko/releases/latest/download/wiktionary-en-ko.zip) |
| [CC-CEDICT-ko](https://github.com/kongchu2/cedict-ko) | 중국어 → 한국어 | 빈도순으로 번역 중 + 한자 훈음 10,353자 | [cedict-ko.zip](https://github.com/kongchu2/cedict-ko/releases/latest/download/cedict-ko.zip) · [hanzi-ko.zip](https://github.com/kongchu2/cedict-ko/releases/latest/download/hanzi-ko.zip) |

## 무엇이 좋은가

- **읽던 자리에서 바로**: 단어 위에서 Shift를 누르면(설정에 따라 마우스만 올려도) 뜻이 뜹니다. 탭을 옮겨 사전을 검색할 필요가 없습니다.
- **활용형을 알아봅니다**: `食べられなかった` → 食べる, `went` → go, `picked it up` → pick up.
- **무료, 광고 없음, 오프라인**: 사전은 브라우저 안에 저장됩니다.
- **Anki 연동**: 찾은 단어를 버튼 하나로 단어 카드로 만듭니다.
- **한국어 화자에게 맞춘 정보**: 한자에는 한국 한자 훈음(`学` 배울 학)이 나옵니다.

## 알고 쓰세요

한국어 뜻은 사람이 쓴 것이 아니라 **LLM(Claude) 자동 번역**입니다. 공개 사전(JMdict, 영어 위키낱말사전, CC-CEDICT)의 표제어와 뜻 구분을 그대로 두고 뜻만 한국어로 옮겼습니다. 오역이 있을 수 있어서 항목마다 영어 원문을 접어 두었고, 모델이 확신하지 못한 항목에는 `※ 자동 번역 신뢰도 낮음` 표시가 붙습니다. 틀린 뜻을 보면 각 사전 저장소의 Issues에 알려 주세요.

## 설치 (5분)

### 1. Yomitan 설치

- [Chrome / Edge / Whale](https://chromewebstore.google.com/detail/yomitan/likgccmbimhjbgkjambclfkhldnlhbnn)
- [Firefox](https://addons.mozilla.org/firefox/addon/yomitan/) (안드로이드 Firefox에서도 됩니다)
- iPhone·iPad·Mac의 Safari는 지원하지 않습니다.

설치하면 환영 페이지가 열립니다. 추천 사전을 묻는 창은 건너뛰어도 됩니다(영어 뜻 사전입니다).

### 2. 언어 고르기

Yomitan 아이콘 → 톱니바퀴(설정) → **General → Language**에서 읽을 언어를 고릅니다(Japanese / English / Chinese).

여러 언어를 읽는다면 **Profiles**에서 언어마다 프로필을 하나씩 만드세요. 한 프로필은 한 언어만 다룹니다.

### 3. 사전 넣기

위 표에서 zip을 받고, 설정의 **Dictionaries → Configure installed and enabled dictionaries → Import**에서 불러옵니다. 압축은 풀지 않습니다. 큰 사전은 몇 분 걸립니다.

### 4. 써 보기

아무 웹페이지에서 단어 위에 마우스를 두고 **Shift**를 누릅니다. 새 버전은 Dictionaries 화면의 업데이트 확인으로 받을 수 있습니다.

## 언어별 권장 설정

**일본어**
- 따로 바꿀 것은 없습니다. 영어 뜻 사전(Jitendex 등)을 함께 넣어 두면 아직 번역되지 않은 드문 단어를 메울 수 있습니다.

**영어**
- **Scanning → Lookup resolution을 Word로** 바꾸세요. 기본값(Letter)에서는 `went` 밑에 `wen`, `we`가 함께 나오고, 숙어가 다음 단어의 앞부분까지 잡는 일이 있습니다.

**중국어**
- 간체와 번체 모두 검색됩니다. 병음은 성조 부호로 나옵니다.
- `hanzi-ko.zip`을 함께 넣으면 뜻 창에서 글자를 눌렀을 때 훈음이 나옵니다.
- 글자가 일본식 자형으로 보이면 [이 CSS](https://github.com/MarvNC/yomitan-dictionaries#yomitan-css-for-non-japanese-cjk-languages)를 Appearance → Custom CSS에 넣으세요.

## 자주 묻는 것

- **뜻이 안 뜹니다.** General → Language가 읽는 글의 언어인지, Dictionaries에서 사전이 켜져 있는지 확인하세요.
- **모바일에서도 되나요?** 안드로이드는 Firefox나 Edge에 Yomitan을 설치하면 됩니다. iOS는 안 됩니다.
- **상업적으로 써도 되나요?** 사전 데이터는 CC BY-SA 4.0입니다. 출처를 밝히고 같은 라이선스로 배포하면 됩니다.
- **오역을 고치고 싶어요.** 각 저장소의 `translations/terms.jsonl`에서 해당 줄을 고쳐 PR을 보내거나, Issues에 단어와 맞는 뜻을 적어 주세요.

---

## English

Korean-definition dictionaries for [Yomitan](https://yomitan.wiki/): Japanese→Korean ([JMdict-ko](https://github.com/kongchu2/jmdict-ko)), English→Korean ([Wiktionary-en-ko](https://github.com/kongchu2/wiktionary-en-ko)) and Chinese→Korean ([CC-CEDICT-ko](https://github.com/kongchu2/cedict-ko)). Each keeps the entries and sense structure of an open dictionary (JMdict, English Wiktionary, CC-CEDICT) and gives every sense in Korean. The Korean glosses are machine-translated with an LLM (Claude); the original English is kept in each entry and low-confidence entries are marked. Data is CC BY-SA 4.0; downloads are in the table above.
