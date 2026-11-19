# Technical review — AI Generation Community portal

Date: 2026-11-19  
Scope: review of the first bilingual static homepage draft. No tests or deployments were run for this review.

## Current state

The draft is a self-contained HTML page with embedded CSS and JavaScript. It presents the community vision, four participation pathways, a first-build loop, and English/Simplified Chinese copy. It has no package dependencies, server, database, or third-party API.

This is a concept and landing-page MVP. It does not yet provide member registration, accounts, user profiles, posts, chat, moderation tools, search, saved projects, or persistent user-generated content. The page does not yet collect or store visitor information.

## Suggested maintainable structure

Keep the first release static and dependency-free. If the page grows, split its inline assets into named files and keep project logs at the repository root, as they are in this branch:

~~~text
/
├── index.html
├── assets/
│   └── community-mark.svg
├── styles/site.css
├── scripts/site.js
├── locales/
│   ├── en.json
│   └── zh-Hans.json
├── .github/
│   ├── ISSUE_TEMPLATE/
│   └── pull_request_template.md
├── DECISIONS.md
├── COMMUNICATION_LOG.md
├── ROADMAP.md
├── TECHNICAL_REVIEW.md
├── README.md
├── CHANGELOG.md
└── vercel.json
~~~

Do not add a framework until a concrete interactive feature needs server behavior.

## Before connecting the domain

- Link a separate Vercel project to the standalone GitHub repository, with project root set to the repository root.
- Keep branch pushes on preview deployments. Leave the production branch and `www.ai-generation.my` untouched during review.
- After Andrew approves the exact release commit, verify domain ownership, DNS records, and HTTPS before attaching the selected domain.
- Record domain attachment and any DNS edits as a separate launch change. A Vercel preview URL does not prove that the custom domain is ready.

## Review and communication trail

For each material change, record the issue, author, PR, commit SHA, reviewer decision, and relevant Vercel preview URL. Use the GitHub issue for scope and acceptance criteria, the PR for source review, commit history for attribution, `COMMUNICATION_LOG.md` for dated instructions and handoffs, and `DECISIONS.md` for lasting choices. Keep the log factual.

Do not merge to the production branch or attach the custom domain until Andrew approves the preview.

## Homepage review items

- The page now includes a keyboard skip link, visible focus rings, and a `prefers-reduced-motion` rule.
- Browser verification, language-switch review, narrow-screen layout, keyboard operation, and contrast review remain pending until the Vercel preview is available.
- If community content becomes dynamic, render user-provided text as text rather than HTML.

## Gate before live community features

Before collecting member or visitor data, define its purpose, audience, data fields, retention, access roles, moderation path, and launch owner. If children may participate, explicitly decide age range, guardian involvement, safety, and privacy requirements before implementation. No account system, database, public posting, chat, or signup form is included in this draft.
