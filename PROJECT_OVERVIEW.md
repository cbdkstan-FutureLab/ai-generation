# AI Generation Community Portal

An independent, bilingual (English / Simplified Chinese) community portal for AI Generation Community in Malaysia.

## Current scope

This first release is a presentation and orientation site. It introduces the community vision, four audience pathways, and a simple learn–make–share loop. Language switching and mobile navigation run in the browser.

The current portal does not provide member accounts, registration, messaging, user-generated content, analytics, a database, or AI APIs. Calls to action navigate within the page; they do not imply a working signup service.

## Run locally

Open `index.html` in a browser. There are no package dependencies or build step.

## Vercel

The repository root is the static deployment root. Connect `cbdkstan-FutureLab/ai-generation` to Vercel as a standalone project named `ai-generation-community`. Pull requests should generate preview deployments. Keep the custom domain detached until Andrew approves the reviewed version.

## Traceability

- `DECISIONS.md` records accepted scope and platform choices.
- `COMMUNICATION_LOG.md` records founder instructions and implementation updates.
- `CHANGELOG.md` records user-visible changes.
- The GitHub issue and pull request provide the durable task and review trail.
- Commits should be small, named, and attributable. Do not put credentials, personal contact lists, or private member data in this repository.

## Review gate

Before connecting `www.ai-generation.my`, Andrew reviews the Vercel preview and approves the exact commit. After approval, attach the domain to the Vercel project, confirm DNS/TLS, and verify both the apex and `www` behavior selected for launch.
