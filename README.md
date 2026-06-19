# AI 제품 및 서비스 확인제 가이드

이 저장소는 **AI 제품 및 서비스 확인제** 대외 공개용 가이드 웹사이트를 관리하기 위한 문서 전용 리포지토리입니다.

문서는 Markdown으로 작성하고, GitHub Pages와 MkDocs Material을 사용해 Notion형 문서 사이트로 공개하는 구성을 전제로 합니다.

## 문서 구성

```text
.
├─ README.md
├─ mkdocs.yml
├─ requirements.txt
├─ docs/
│  ├─ index.md
│  ├─ overview.md
│  ├─ criteria-summary.md
│  ├─ application-prep.md
│  ├─ criteria/
│  ├─ cases/
│  ├─ appendix/
│  ├─ faq.md
│  └─ public-release-checklist.md
└─ .github/workflows/deploy.yml
```

## 로컬 미리보기

Python이 설치된 환경에서 아래 명령으로 문서 사이트를 미리 볼 수 있습니다.

```bash
pip install -r requirements.txt
mkdocs serve
```

브라우저에서 `http://127.0.0.1:8000`으로 접속합니다.

## GitHub Pages 배포

1. GitHub에 새 public repository를 생성합니다.
2. 이 폴더의 파일을 그대로 업로드합니다.
3. 저장소의 **Settings > Pages**에서 Source를 **GitHub Actions**로 설정합니다.
4. `main` 브랜치에 push하면 `.github/workflows/deploy.yml`이 실행되어 사이트가 배포됩니다.

## 공개 전 주의사항

- API Key, Access Token, 내부 URL, 개인정보, 비공개 담당자 연락처는 공개 저장소에 포함하지 마세요.
- 확인 기준과 법적 근거는 공개 전 담당 부서 검토를 거치세요.
- 이 문서는 대외 공개용 초안입니다. 기관 공식 문서로 게시하기 전 문구, 로고, 저작권, 문의처를 확정해야 합니다.
