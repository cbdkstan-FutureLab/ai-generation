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


## 2026-11-20 — Homepage design direction

- **Founder feedback:** The first CGI felt too simple and not exciting enough to attract members; Andrew asked that the design take inspiration from malaysian.ai.
- **Design response:** Prepared a more energetic concept with a Malaysian skyline and community-learning scene, editorial typography, family activities, project showcases, and event cards. This borrows high-level storytelling patterns only; it does not copy their brand or claim events, testimonials, numbers, or safeguards that are not verified.
- **Design principle:** Parents and educators are the main entry audience; child participation is adult-guided. English, Simplified Chinese, and Bahasa Melayu remain equally supported. Membership is free; no payment gateway is planned. Verified events and community work should make the page feel active.
- **GitHub record:** Added DESIGN_PRINCIPLES.md on branch design/parent-first-trilingual-community (commit b4db70b). This is documentation and concept design only; the live homepage and production domain have not been changed. Pull request will carry the review trail.


## 2026-11-20 — Student-first, content-first homepage revision

- **Founder feedback:** Use CGI images of students and young people only; do not show parents in the images. Represent Chinese, Malay, Indian, and other backgrounds, including Western, European, and African youth, across ages 5–20. Expand the landing page so it explains why the community exists, who will meet and learn together, and what activities people can do together before asking visitors to join.
- **Design response:** Replaced the parent-led hero concept with student-only CGI and a fuller, mission-led page sequence: why we are here; who you will meet; proposed AI discovery labs, build challenges and project showcases; community commitments; then a join invitation. The hero action is “Explore activities.” Guardian guidance for participants under 18 remains in the text and participation principles, not in the CGI.
- **Activity accuracy:** These are proposed activity formats, not confirmed events. Do not publish dates, hosts, partners, outcomes or testimonials until verified. The generated artwork is a CGI concept, not a photograph of actual members or proof of current programmes.
- **Traceability:** Updated DESIGN_PRINCIPLES.md in commit d1e9721 on design/parent-first-trilingual-community and retained the same open review PR #4. No homepage source or production domain was changed by this documentation update.
