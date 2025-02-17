# 음성 인식 및 감정 분석 파이썬 스크립트

## 개요
이 파이썬 스크립트는 구글의 음성 인식 API와 네이버의 감정 분석 API를 사용하여 말한 언어를 텍스트로 변환하고 그 감정을 분석합니다. 마이크를 통해 오디오를 캡처하고 말한 단어의 감정적 톤을 판단하는 간단한 인터페이스를 제공합니다.

## 기능
- **음성 인식:** 구글 음성 인식을 사용하여 말한 언어를 텍스트로 변환합니다.
- **감정 분석:** 네이버의 감정 분석 API를 사용하여 인식된 텍스트의 감정을 분석합니다. 
- **오류 처리:** 사용자에게 명확한 피드백을 제공하면서 타임아웃 및 오류를 관리합니다.

## 요구 사항
- Python 3.x
- `speech_recognition` 라이브러리
- `requests` 라이브러리
- `json` 라이브러리

## 사용 방법
1. 필요한 라이브러리를 설치합니다.
   ```
   pip install speechrecognition requests
   ```
2. 스크립트를 실행하기 전에 네이버 API의 클라이언트 ID와 클라이언트 비밀번호를 설정합니다. https://guide.ncloud-docs.com/docs/clovasentiment-use
3. 터미널이나 커맨드 라인에서 스크립트를 실행하여 음성 인식과 감정 분석을 시작합니다.
4. 스크립트가 실행되면, "말씀하세요!"라는 메시지와 함께 사용자의 음성을 듣기 시작합니다.
5. 음성이 인식되면, 텍스트로 변환된 결과와 감정 분석 결과를 출력합니다.

## 주의 사항
- 음성 인식 정확도는 사용 환경과 발음에 따라 달라질 수 있습니다.
- API 키는 보안을 위해 안전하게 관리해야 합니다.
- 네트워크 연결 상태에 따라 API 응답 시간이 달라질 수 있습니다.
