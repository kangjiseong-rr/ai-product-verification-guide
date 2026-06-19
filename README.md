# AI 제품 및 서비스 확인제 가이드

대외 공개용 문서 사이트로 운영하기 위한 MkDocs Material 기반 가이드입니다.

## 구성

```text
.
├─ mkdocs.yml
├─ requirements.txt
├─ docs/
│  ├─ index.md
│  ├─ 00-source-map.md
│  ├─ 01-overview.md
│  ├─ 02-criteria.md
│  ├─ review-guide/
│  ├─ 03-cases.md
│  ├─ 04-recognized-ai-models.md
│  ├─ 05-original-pages.md
│  ├─ 06-publication-checklist.md
│  └─ assets/
└─ .github/workflows/deploy.yml
```

## 로컬 실행

```bash
pip install -r requirements.txt
mkdocs serve
```

브라우저에서 `http://127.0.0.1:8000` 접속

## GitHub Pages 배포

1. GitHub에 새 public repository 생성
2. 이 폴더의 파일 전체 업로드
3. `main` 브랜치에 push
4. GitHub Actions 실행 후 `gh-pages` 브랜치 생성 확인
5. Repository Settings > Pages에서 배포 소스를 `gh-pages` 브랜치로 설정

## 주의

- 본 패키지는 업로드된 PDF 원문을 공개용 문서 사이트 구조로 재구성한 초안입니다.
- 대외 공개 전 기관명, 담당자 정보, 내부 검토 표현, API Key 예시, 보안상 민감한 이미지 또는 로그는 반드시 검토하세요.
- `docs/05-original-pages.md`에는 원문 누락 방지를 위해 PDF 페이지 렌더링 이미지를 포함했습니다. 공개 범위에 따라 유지 또는 삭제하세요.
