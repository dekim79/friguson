# FRIGUSON 홈페이지

㈜프리거슨(FRIGUSON) 공식 홈페이지 소스입니다. [Jekyll](https://jekyllrb.com/)로 만들어졌고, **GitHub Pages**에 올리면 별도의 빌드 서버 없이 자동으로 배포됩니다.

- 한국어: `/` (사이트 루트)
- English: `/en/`
- Experimental World 글: `_experiments_ko/`, `_experiments_en/` 폴더

콘텐츠(글, 사진, 연락처 등)를 직접 업데이트하는 방법은 **[CONTENT_GUIDE.md](CONTENT_GUIDE.md)** 를 참고하세요. 코드를 몰라도 GitHub 웹사이트에서 바로 수정할 수 있도록 정리했습니다.

## 폴더 구조

```
web_page/
├── index.md, about.md, technology.md, lab-solutions.md,
│   experimental-world.md, contact.md   ← 한국어 페이지
├── en/                                  ← 영어 페이지 (동일 구조)
├── _experiments_ko/                     ← Experimental World 글 (한국어)
├── _experiments_en/                     ← Experimental World 글 (영어)
├── _layouts/, _includes/                ← 페이지 뼈대(템플릿)
├── _data/nav.yml                        ← 상단 메뉴 구성
├── assets/images/                       ← 로고, 사진, 다이어그램
├── assets/css/style.css                 ← 디자인(색상, 레이아웃)
├── _config.yml                          ← 사이트 전체 설정
└── CONTENT_GUIDE.md                     ← 콘텐츠 업데이트 가이드
```

## GitHub Pages로 배포하기

1. GitHub에 새 저장소를 만들고 이 폴더 전체를 업로드(push)합니다.
2. 저장소 **Settings → Pages** 로 이동합니다.
3. **Source**를 "Deploy from a branch"로, 브랜치를 `main`(또는 기본 브랜치), 폴더를 `/ (root)`로 설정합니다.
4. 잠시 후 `https://<사용자명>.github.io/<저장소이름>/` 주소로 사이트가 열립니다.
5. `_config.yml`의 `url`과 `baseurl` 값을 실제 주소에 맞게 수정한 뒤 다시 push하세요.
   - `사용자명.github.io` 형태의 개인/조직 페이지라면 `baseurl: ""`
   - `사용자명.github.io/저장소이름` 형태의 프로젝트 페이지라면 `baseurl: "/저장소이름"`
6. 커스텀 도메인(예: `friguson.com`)을 연결하려면 저장소 루트에 `CNAME` 파일을 추가하고, GitHub Pages 설정에서 도메인을 등록하세요.

GitHub Pages는 `main` 브랜치에 push될 때마다 자동으로 사이트를 다시 빌드합니다. 별도의 GitHub Actions 설정이 필요 없습니다.

## 로컬에서 미리보기 (선택사항)

Ruby가 설치되어 있다면 아래 명령으로 로컬에서 확인할 수 있습니다.

```bash
bundle install
bundle exec jekyll serve
```

브라우저에서 `http://localhost:4000` 으로 접속하면 됩니다. 로컬 미리보기 없이 GitHub Pages에 바로 올려서 확인해도 됩니다.

## 원본 자료 안내

`assets/images/`의 로고, 다이어그램 이미지는 제공해주신 로고 파일과 사업계획 발표자료(PDF)에서 발췌·가공한 것입니다. 발표자료 원본 PDF에는 예산·매출 등 내부 정보가 포함되어 있어 저장소에는 포함하지 않았습니다. 필요 시 별도로 보관하세요.
