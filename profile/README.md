# Hir3d

**AI-powered recruiting and candidate discovery.**

Hir3d helps recruiting teams analyze resumes, discover candidates, and streamline hiring workflows with AI. This organization is a maintained portfolio of the Hir3d hiring platform.

[Learn More](https://me.x70.one/work/hir3d) · [dan@x70.one](mailto:dan@x70.one)

---

## Repositories

| Repository | Role | Live |
| --- | --- | --- |
| [web](https://github.com/hir3d-one/web) | Marketing and portfolio site | [hir3d-web.vercel.app](https://hir3d-web.vercel.app) |
| [app](https://github.com/hir3d-one/app) | Recruiter dashboard — search, review, orgs, API keys, jobs | [hir3d-app.vercel.app](https://hir3d-app.vercel.app) |
| [upload](https://github.com/hir3d-one/upload) | Candidate portal — CV upload and analysis review | [hir3d-upload.vercel.app](https://hir3d-upload.vercel.app) |
| [cli](https://github.com/hir3d-one/cli) | Dev CLI for CV ingestion and candidate search | — |

## Stack

- **Apps:** Next.js, React, TypeScript, Tailwind CSS
- **Auth & data:** Better Auth, Prisma, MySQL
- **AI:** Vercel AI SDK, Google Gemini
- **Jobs:** Trigger.dev
- **Storage:** Azure Blob Storage
- **Tooling:** pnpm, Turborepo, Node.js 22

## Architecture

```text
Candidates ──► upload ──► CV analysis (Gemini) ──► MySQL + Blob
                              │
Recruiters ──► app ───────────┴──► AI search & ranking
                              │
Developers ──► cli ───────────┘
```

## Note

The original `hir3d.one` domain is inactive. Live demos run on Vercel via the links above.
