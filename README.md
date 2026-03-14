# Astro 블로그 스타터 키트

```sh
npm create astro@latest -- --template blog
```

> 🧑‍🚀 **숙련된 우주비행사?** 이 파일을 삭제하세요. 즐기세요!

기능:

- ✅ 최소한의 스타일링 (자신만의 것으로 만드세요!)
- ✅ 100/100 Lighthouse 성능
- ✅ 표준 URL과 Open Graph 데이터로 SEO 친화적
- ✅ 사이트맵 지원
- ✅ RSS 피드 지원
- ✅ Markdown & MDX 지원

## 🚀 프로젝트 구조

Astro 프로젝트 내부에서 다음과 같은 폴더와 파일을 볼 수 있습니다:

```text
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── layouts/
│   └── pages/
├── astro.config.mjs
├── README.md
├── package.json
└── tsconfig.json
```

Astro는 `src/pages/` 디렉토리에서 `.astro` 또는 `.md` 파일을 찾습니다. 각 페이지는 파일 이름에 따라 경로로 노출됩니다.

`src/components/`에는 특별한 것이 없지만, Astro/React/Vue/Svelte/Preact 컴포넌트를 넣는 곳입니다.

`src/content/` 디렉토리에는 관련 Markdown 및 MDX 문서의 "컬렉션"이 포함됩니다. `getCollection()`을 사용하여 `src/content/blog/`에서 게시물을 검색하고, 선택적 스키마를 사용하여 프론트매터를 타입 체크하세요. 자세한 내용은 [Astro의 콘텐츠 컬렉션 문서](https://docs.astro.build/en/guides/content-collections/)를 참조하세요.

이미지와 같은 정적 자산은 `public/` 디렉토리에 배치할 수 있습니다.

## 🧞 명령어

모든 명령어는 프로젝트 루트의 터미널에서 실행됩니다:

| 명령어                    | 동작                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | 의존성 설치                                     |
| `npm run dev`             | `localhost:4321`에서 로컬 개발 서버 시작        |
| `npm run build`           | `./dist/`에 프로덕션 사이트 빌드                 |
| `npm run preview`         | 배포 전에 로컬에서 빌드 미리보기                 |
| `npm run astro ...`       | `astro add`, `astro check` 같은 CLI 명령어 실행 |
| `npm run astro -- --help` | Astro CLI 사용 도움말 얻기                       |

## 👀 더 배우고 싶으신가요?

[문서](https://docs.astro.build)를 확인하거나 [Discord 서버](https://astro.build/chat)에 참여하세요.

## 크레딧

이 테마는 멋진 [Bear Blog](https://github.com/HermanMartinus/bearblog/)를 기반으로 합니다.
