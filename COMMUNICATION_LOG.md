# Communication and handoff log


This file records material project instructions and implementation decisions. GitHub issue and pull request timestamps plus commit history remain the primary event trail. Do not add private credentials or personal member data here.


## 2026-11-19 — Founder kickoff


- **Request:** Start building the AI community portal tonight.
- **Platform direction:** Use GitHub and Vercel; keep the project standalone.
- **Traceability:** Keep source code, decisions, changes, and communication trail reviewable.
- **Launch gate:** Prepare for `www.ai-generation.my`, but attach the official domain only after Andrew approves the reviewed version.
- **Implementation response:** Create a bilingual static orientation portal as the first reviewable slice. Keep membership, chat, registration, and user-generated content out of scope until requirements and governance are agreed.


## Handoffs


- Engineering work should be linked to the GitHub issue and PR. Use the PR for review comments and the decision log for lasting outcomes.
- No message has been sent through an external Tim account; the engineering review in this workspace was completed by the local Tim delegate.


## 2026-11-19 — Delivery approach clarified


- **Founder instruction:** Use GitHub and Vercel; keep the portal independent from other repositories; make all source and communication traceable; prepare for immediate domain hookup after approval.
- **Work plan:** Use the founder-created public standalone repository `cbdkstan-FutureLab/ai-generation`, a separate Vercel project, and review deployments. Record Andrew’s approval against the exact commit before any domain is attached.
- **Platform finding:** The connected Vercel team is `AndrewTeam`; its visible domain inventory includes `futurelab.com.my` but not `ai-generation.my`. Registrar and DNS readiness must be confirmed before promising a same-night domain cutover.
- **Tim handoff:** The local engineering review is saved in `TECHNICAL_REVIEW.md`. No message was sent through an external Tim account.
- **Engineering review:** The local Tim delegate reviewed the draft. Keyboard focus and reduced-motion styles were then added to the page. Browser verification remains pending.

## 2026-11-19 — Trilingual launch and domain instruction

- **Founder instruction:** Provide English, Mandarin, and Malay, and connect the portal to `www.ai-generation.my` now. This is Andrew's approval to merge and publish the portal.
- **Language update:** Added a three-option language selector, full page copy in all three languages, and saved language preference. Source commit: `2fcabe89cd1e3a407092f64320f7003c5e1aa985`.
- **Domain check:** Vercel reports the domain is on external MSCHosting nameservers and currently misconfigured for this project; the existing apex A record is `103.7.9.22`. The exact `www` CNAME will be recorded after adding the domain to the Vercel project.
- **Publishing step:** Merge the approved branch to `main`; if MSCHosting DNS cannot be changed through a connected account, provide Andrew the precise record to add.
