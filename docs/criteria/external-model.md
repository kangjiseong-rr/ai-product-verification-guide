# 외부 모델 연동 확인

외부 모델 연동 확인은 OpenAI, Anthropic, Google, 네이버클라우드, LG AI연구원 등 외부 AI 서비스를 사용하는 경우 실제 연동 여부를 확인하는 영역입니다.

## 항목 3.1 API 연동

**질문:** 외부 모델 연동 시 호출 로그나 API Key가 존재하는가?

### 서류 확인 관점

신청서에는 외부 모델 연동 여부가 명확히 표시되어야 합니다.

다음과 같은 서비스 사용 여부를 확인할 수 있습니다.

- OpenAI
- Anthropic
- Google Generative AI
- 네이버클라우드 HyperCLOVA X
- LG AI연구원 등 국내외 AI 서비스
- 기타 상용 또는 오픈소스 기반 외부 AI 모델 API

### 현장 확인 관점

다음과 같은 연동 흔적을 확인할 수 있습니다.

- AI 기능 실행 시 호출 로그가 추가되는지 확인
- 외부 API 호출 시점과 제품 기능 실행 시점이 일치하는지 확인
- API Key 또는 인증 설정이 존재하는지 확인
- 외부 AI 서비스 호출 결과가 제품의 핵심 기능에 반영되는지 확인

### 판정 방향

아래에 해당하면 통과 가능성이 있습니다.

- 알려진 AI 서비스를 활용하고, 호출 로그 또는 API Key 등 연동 증빙을 확인할 수 있음

!!! danger "공개 문서 작성 시 주의"
    API Key 원문은 공개 문서나 공개 저장소에 절대 포함하지 마세요. 예시 화면에는 `sk-****`, `Bearer ****`처럼 마스킹된 값을 사용해야 합니다.

## 예시 로그 표현

```text
[INFO] [AI-FUNCTION] Start AI function execution
[INFO] [EXTERNAL-AI-CALL] Calling external API: OpenAI GPT
[DEBUG] [OpenAI-Client] POST https://api.example.com/v1/chat/completions
[DEBUG] [OpenAI-Client] Authorization: Bearer sk-********
```

위 예시는 형식 설명을 위한 샘플입니다. 실제 운영 로그를 공개할 때는 URL, 토큰, 사용자 식별자, 파일명, 내부 경로 등을 반드시 마스킹해야 합니다.
