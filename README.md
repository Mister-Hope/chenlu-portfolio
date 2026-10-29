# Chen Lu · Portfolio

> [🇨🇳 中文版](./README.zh-CN.md)

Personal portfolio and résumé site of **Chen Lu (陈璐)** — a Ph.D. candidate in condensed matter physics at Northeast Normal University, currently seeking a **high school physics teaching position**.

The site is bilingual: English at `/`, Chinese at `/zh/`.

## About

- Integrated bachelor–master–doctoral training in physics at Northeast Normal University, admitted through the recommendation-without-examination track.
- Four years of high school physics teaching and teaching-research practice; familiar with the high school physics curriculum and key exam points.
- Six consecutive years of student leadership: undergraduate grade leader, graduate grade coordinator and student union secretary-general.
- First-author publications in _Light: Science & Applications_, _Physical Review Research_ and _J. Mater. Chem. C_.

## Site Sections

| Section                | Content                                                       |
| ---------------------- | ------------------------------------------------------------- |
| Profile                | Basic information, certificates and contact details           |
| Career Aspiration      | Teaching-oriented objective and call to action                |
| Education & Experience | Degrees, teaching roles, volunteer work and research projects |
| Selected Publications  | First-author and co-first-author papers with journal tiers    |
| Academic Collaboration | Co-authored publications                                      |
| Honors & Awards        | Scholarships, honors and competitions                         |
| Student Work           | Leadership roles and responsibilities                         |
| Self-Evaluation        | Summary of strengths and commitment to teaching               |

## Local Development

```bash
pnpm ci          # install dependencies
pnpm run dev     # start the dev server at http://localhost:3000
pnpm run build   # type-check and build to dist/
pnpm run preview # preview the production build
pnpm run lint    # lint and format
```

## Editing Content

All user-facing content lives in [`config.yml`](./config.yml), organized by locale (`/` for English, `/zh/` for Chinese). No source changes are needed for content updates.

- Text, links, sections, media → `config.yml`
- Style fine-tuning → `custom.css` in the project root (auto-injected at build time)
- Full configuration reference → [`docs/en.md`](./docs/en.md) / [`docs/zh.md`](./docs/zh.md)

## Deployment

Every push to `main` runs the `Deploy Docs` GitHub Actions workflow, which builds the site and publishes `dist/` to the `gh-pages` branch for GitHub Pages. The same `dist/` output can be hosted on Vercel, Netlify or any static file server.

## Tech Stack

- React 19 + Vite 8, TypeScript
- Tailwind CSS v4
- Iconify icons
- Markdown rendering with markdown-it and static site generation via a custom Vite plugin

## Project Structure

```text
.
├── config.yml          # All site content (English + Chinese)
├── custom.css          # Custom style overrides, auto-injected
├── public/             # Static assets (avatar, background)
├── src/                # React components and styles
├── lib/                # Config loader, Markdown renderer, SSG plugin
├── docs/               # Configuration reference
└── examples/           # Example configs in other formats
```

## Contact

- Email: [chenl987@nenu.edu.cn](mailto:chenl987@nenu.edu.cn)
- ORCID: [0009-0006-5397-4679](https://orcid.org/0009-0006-5397-4679)
- Résumé: <https://chenlu-resume.innenu.com>
