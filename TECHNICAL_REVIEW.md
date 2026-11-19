# Technical review — AI Generation Community portal

Date: 2026-11-19  
Scope: review of the first bilingual static homepage draft. No tests or deployments were run for this review.

## Current state

The draft is a self-contained HTML page with embedded CSS and JavaScript. It presents the community vision, four participation pathways, a first-build loop, and English/Simplified Chinese copy. It has no package dependencies, server, database, or third-party API.

This is a concept and landing-page MVP. It does not yet provide member registration, accounts, user profiles, posts, chat, moderation tools, search, saved projects, or persistent user-generated content. The page does not yet collect or store visitor information.

## Recommended standalone structure

Keep the first release static and dependency-free. Before ongoing feature work, move the current inline assets into named files so reviews and changes remain easy to trace:

~~~~text
/
├── index.html
├── assets/
│   └── community-mark.svg
├── styles/
│   └── site.css
├── scripts/
│   └── site.js
├── locales/
│   ├── en.json
│   └── zh-Hans.json
├── docs/
│   ├── DECISIONS.md
│   ├── COMMUNICATION_LOG.md
│   ├── ROADMAP.md
│   └── TECHNICAL_REVIEW.md
├── .github/
│   ├── ISSUE_TEMPLATE/
│   └── pull_request_template.md
├── README.md
├── CHANGELOG.md
└── vercel.json
~~~~

The file split can be done in the first reviewable pull request; do not add a framework until a concrete interactive feature needs server behavior.

## Before connecting the domain

- Create a Vercel project linked to the standalone GitHub repository, with the project root set to the repository root.
- Keep branch pushes on preview deployments. Keep the production branch and www.ai-generation.my untouched during review.
- Once Andrew approves the release, verify the Vercel project, domain ownership, DNS records, and HTTPS status, then attach the selected domain and promote the approved version.
- Keep domain attachment and any DNS edits in a separately recorded launch change. A Vercel preview URL is not proof that the custom domain is ready.

## Review and communication trail

For each material change, record the issue, author, PR, commit SHA, reviewer decision, and relevant Vercel preview URL. Use:

1. A GitHub issue as the scoped work request and acceptance checklist.
2. A pull request for source review, with its preview URL and screenshots if available.
3. The commit history for source-level change attribution.
4. docs/COMMUNICATION_LOG.md for dated project decisions and handoffs; keep it factual and do not invent conversations.
5. docs/DECISIONS.md for durable product or architecture choices, with the deciding person and date.

Do not merge to the production branch or attach the custom domain until the user approves the preview.

## Homepage quality items for the review pass

- Format the embedded CSS and JavaScript before adding more page content.
- Add visible :focus-visible states and a prefers-reduced-motion rule.
- Verify keyboard operation and narrow-screen layout; confirm both language versions fit without overflow.
- Keep the current language strings static. If community content becomes dynamic, render user-provided text as text, not HTML.
- Review colour contrast on the dark palette before sign-off.

## Gate before live community features

Before adding any feature that accepts member or visitor data, define its audience, data fields, retention, access roles, moderation path, and launch owner. No authentication, database, public posting, messaging, or signup form is included in the current draft. If children may participate, make age range, guardian involvement, safety and privacy requirements an explicit product decision before implementation.

## Release acceptance checklist

- [ ] Scope and audience approved.
- [ ] English and Simplified Chinese copy reviewed.
- [ ] Mobile and desktop preview reviewed.
- [ ] Keyboard access and reduced-motion behavior reviewed.
- [ ] Source changes reviewed in a GitHub PR; commit and preview URL recorded.
- [ ] Vercel project is linked to this standalone repository.
- [ ] User approves production release.
- [ ] Domain and DNS configuration verified before attaching www.ai-generation.my.

## Changes made after this review

- Added a keyboard skip link, visible focus rings, and a `prefers-reduced-motion` rule.
- Browser verification, language-switch review, and mobile layout review remain pending until the Vercel preview is available.
