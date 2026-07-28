# 탁류 인터랙티브 문학기행

채만식의 소설 「탁류」의 배경인 전북 군산을 답사하는 인터랙티브 웹앱입니다. AI 스튜디오(Google AI Studio) 연수용 실습 2번 자료로 제작되었습니다.

## 파일 구조

| 파일 | 설명 |
|---|---|
| `index_takryu.html` | 탁류 전용 단순화 버전 (메인 진입점) |
| `index.html` | 원본 (10개 지역/작품 전체 버전, 참고용) |
| `map_all.html` | 전체 코스 지도 |
| `map_emotional.html` | 감성 여행자 코스 지도 (콩나물 고개, 월명산) |
| `map_intellectual.html` | 지성 여행자 코스 지도 (금강, 은행 거리, 미두장) |
| `map_realist.html` | 리얼리스트 코스 지도 (개복동, 역전시장) |
| `docs/AI스튜디오_연수_통합가이드.docx` | 연수 통합 가이드 (API 키 발급, 실습 프롬프트, 진행 타임테이블, 트러블슈팅) |

지도 파일들은 Colab + folium으로 미리 생성한 정적 HTML이며, `index_takryu.html`에서 iframe으로 불러옵니다.

## 실행 방법

**로컬에서 열기**: `index_takryu.html`을 브라우저로 엽니다. `map_*.html` 4개가 같은 폴더에 있어야 지도가 정상적으로 표시됩니다.

**AI 스튜디오(AI Studio Build)에서 편집하기**:
1. `index_takryu.html`과 `map_all.html`, `map_emotional.html`, `map_intellectual.html`, `map_realist.html` 5개 파일을 프로젝트에 함께 업로드
2. `docs/AI스튜디오_연수_통합가이드.docx`의 "실습 2" 섹션에 있는 안내 프롬프트를 채팅창에 붙여넣기
3. 이후 원하는 커스터마이징을 프롬프트로 요청

## 앱 흐름

여행 시작 → 표지 클릭 → 페르소나 테스트(심리테스트 링크 + 3개 코스 카드) → 선택한 코스의 지도와 소설 속 인용문 표시

## 배경

25명 대상 AI 리터러시 연수의 실습 자료 중 하나입니다 (실습 1: MBTI 도서 추천 앱, 알라딘 Open API 연동).
