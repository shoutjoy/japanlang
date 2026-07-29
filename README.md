# 일본어 AI 학습 스튜디오

## 실행
```bash
npm install
npm run dev
```

## 주요 기능
- 모바일 히라가나·가타가나 문자표
- 설치된 일본어 음성 중 고품질 음성을 선택하는 자연스러운 TTS
- VOICEVOX(`127.0.0.1:50021`) 완전 로컬 AI 음성과 화자 선택
- Google AI Studio API Key 연결 시 Gemini AI 음성 읽기
- 시작 버튼과 이동 가능한 큰 글자 읽기 팝업
- 읽기 정지 후 현재 글자부터 이어 읽기 및 이전·다음 글자 이동
- KanjiVG 기반 실제 획순을 1획씩 재생하는 쓰기 애니메이션
- 읽는 문자와 짝이 되는 히라가나·가타가나 동시 표시
- 기본 오십음도별 읽기 횟수 누적·IndexedDB 저장
- 쓰기 연습, 단어 시험, 혼합 게임, 문자 퀴즈
- IndexedDB 학습기록·추가 단어·AI 설정 저장
- XLSX·CSV 단어 가져오기와 기록 XLSX 내보내기
- LM Studio OpenAI 호환 API 및 Google AI Studio Gemini API
- AI 문제 생성, 한국어→일본어 번역, 예문·학습 챗

## 파일 열
필수: `일본어`, `한국어`
선택: `읽기`, `로마자`, `한국어읽기`

## 보안
브라우저에 API Key를 저장하는 방식은 개인 로컬 사용에만 적합합니다.
공개 배포 시에는 서버 프록시에서 API Key를 관리하십시오.

## VOICEVOX
VOICEVOX 앱 또는 `vv-engine/run.exe`를 실행하면 앱이 로컬 엔진을 자동 감지합니다.
Windows에서는 `winget install --id HiroshibaKazuyuki.VOICEVOX`로 GPU/DirectML판을 설치할 수 있습니다.

## 획순 데이터
히라가나·가타가나 실제 획순은 KanjiVG `r20250816` 데이터를 사용합니다.
데이터 라이선스와 출처는 `public/strokes/ATTRIBUTION.md` 및 `public/strokes/COPYING`에 포함되어 있습니다.
