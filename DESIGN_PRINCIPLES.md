# AI Generation Community — Design Principles

**Status:** Founder-approved product direction; implementation requirements remain gated until built and reviewed.  
**Owner:** Andrew Tan  
**Last updated:** 2026-11-20 (Malaysia time)

This document guides the portal's content, user experience, and future membership features. It does not claim planned safeguards or account features already exist.

## 1. Purpose and audience

AI Generation Community is a free, non-commercial Malaysian community where young people aged 5–20 explore artificial intelligence, create useful projects, and learn alongside peers, educators, mentors, makers, and people working with AI. The community welcomes Chinese, Malay, Indian, and other backgrounds, including international, European, and African learners.

The first page must earn attention with a clear purpose and meaningful activities before inviting visitors to join. Speak directly to young people while making the role of educators and trusted adults clear. Participants under 18 require age-appropriate, adult-guided participation; do not position a child as an independent account holder.

## 2. Safe, age-appropriate participation

Every youth-facing invitation should explain what participants can learn or make, what adult guidance is expected for minors, what data is collected and why, how sharing and contact work, and how reporting, moderation, and deletion are handled.

Future child participation must default to adult-led registration and guardian oversight, no public child profile, no unsolicited direct messaging, and parent or guardian review before a child's work is made public. Community rules, reporting, and an operating moderation process must be ready before member interaction or user-generated content is enabled. Collect the minimum information needed; prefer a nickname and age band over full name, exact birth date, school, phone, or address.

These are implementation requirements, not claims about current functionality. Do not promise moderation or safety controls until they are live and staffed.

## 3. First-page experience

The landing page must have enough substance to answer, before any join prompt:

1. **Why we exist:** AI is changing how people learn, work, and create; young Malaysians should have a welcoming place to understand it and shape what comes next.
2. **Who we bring together:** learners aged 5–20, educators, mentors, makers, families, and AI practitioners. Do not imply a partner or named person is confirmed until verified.
3. **What we do together:** proposed formats include age-appropriate AI discovery sessions, hands-on build labs, responsible-AI conversations, team challenges, creator showcases, and talks with practitioners. Label these as planned until dates, hosts, and delivery are confirmed.
4. **How participation works:** explain suitable age groups, adult guidance for under-18s, and community expectations.
5. **Trust and next steps:** make the rules and privacy information easy to find, then invite visitors to explore or join through a flow that is actually implemented.

Use this page order: **Purpose → People → Activities → Community expectations → Join**. The first action after the hero should be **Explore activities**. Place the main **Join the community** invitation after visitors understand the offer. Do not ask people to join before the page has shown why it matters.

### Homepage copy draft

| English | 中文 | Bahasa Melayu |
|---|---|---|
| **AI is shaping tomorrow. Let’s build it together.** A Malaysian community for young people aged 5–20 to explore AI, make things that matter, and learn alongside peers, educators, mentors and people building with AI. | **人工智能正在塑造未来。让我们一起创造。** 一个属于马来西亚 5–20 岁年轻人的社区，与同伴、教育工作者、导师和 AI 实践者一起认识人工智能、动手创造有意义的作品。 | **AI sedang membentuk masa depan. Mari kita bina bersama.** Komuniti Malaysia untuk golongan muda berumur 5–20 tahun meneroka AI, menghasilkan sesuatu yang bermakna dan belajar bersama rakan sebaya, pendidik, mentor serta pengamal AI. |
| **Explore activities** · **Meet the community** | **探索活动** · **认识我们的社群** | **Terokai aktiviti** · **Kenali komuniti kami** |
| **Join the community** — show this invitation after the purpose, people and activities are clear. | **加入社群** — 先介绍宗旨、参与者和活动，再邀请加入。 | **Sertai komuniti** — jemput pelawat selepas tujuan, peserta dan aktiviti diterangkan. |
| **Free to join · No payment required** | **免费加入 · 无需付款** | **Pendaftaran percuma · Tiada bayaran diperlukan** |

### Proposed activity themes

Use these as clear examples of what members may do together, not as confirmed events or promises until delivery is arranged:

- **Discover AI:** age-appropriate introductions to how AI works and where people encounter it.
- **Build with AI:** guided creative challenges using accessible tools and materials.
- **Think responsibly:** discuss fairness, privacy, safety, and the effect of AI on people.
- **Make it together:** collaborate across ages and backgrounds on practical projects.
- **Show what you made:** share projects in an appropriately moderated showcase after approval and consent processes are in place.
- **Meet people in AI:** invite educators, makers, researchers, and practitioners when hosts are confirmed.

## 4. Language parity

English, Simplified Chinese, and Bahasa Melayu are first-class experiences. Core navigation, calls to action, youth and guardian guidance, privacy notices, and community rules must be available in all three languages. Switching languages must not interrupt the visitor's journey or silently reset their selection.

## 5. Visual direction

Build a bold, editorial, Malaysia-rooted experience with a rich, immersive first page, confident typography, warm cream and forest-green accents, and clear pathways into purpose, people, activities, and community stories. The CGI hero must feature students and young people only—no parents or adults in the student hero imagery. Represent Chinese, Malay, Indian, and other learners, including Western, European, and African backgrounds, across the 5–20 age range. Show varied ages naturally and respectfully; avoid tokenistic grouping.

The full page should use real student-led learning and project imagery where available, then activity cards, a “who you’ll meet” section, community outcomes, and a join invitation after the content. Build energy through meaningful work and collaboration rather than decorative AI graphics alone. Show only verified events, projects, partners, testimonials, and impact; label proposed programmes as planned. Keep text accessible and mobile-friendly. Use CGI concept art only when identified as concept art; do not imply unbuilt features or protections. Official logo, colors, and brand assets remain subject to founder approval.

### Landing page content sequence

1. Hero: mission-led headline, student-only CGI, and **Explore activities**.
2. Why this community exists: practical AI literacy, creativity, confidence, and responsible use.
3. Who we bring together: students aged 5–20, educators, mentors, makers, and AI practitioners.
4. What we do: proposed AI discovery, hands-on labs, team challenges, responsible-AI discussions, project showcases, and practitioner sessions. Publish schedules only after confirmation.
5. What members can learn or create: examples must be realistic and clearly framed as examples until delivered.
6. Community commitments: inclusion, respectful collaboration, age-appropriate guidance, and privacy.
7. Join invitation: explain eligibility and the actual sign-up process; keep parent or guardian guidance for under-18 participation visible.

## 6. Membership, authentication, and data

A static information site does not need a database. Once people can create accounts, log in, save profiles, join activities, or have participation records, the portal needs authentication and a database.

- **Phase 1 — Orientation:** Public trilingual information, community rules, privacy information, and an adult interest/contact path. No child accounts.
- **Phase 2 — Adult member accounts:** Verified email sign-in (magic link or equivalent) and minimal membership records. Evaluate Supabase Auth plus Postgres as the initial option.
- **Phase 3 — Parent-managed child participation:** Add only after guardian consent, access control, moderation, retention/deletion, and parent-access workflows are designed and reviewed.

Store only data needed for each phase. When consent is required, record its purpose, notice version, and timestamp. Provide a way to access, correct, and request deletion of member data. Keep credentials and personal member records out of this public source repository.

## 7. Free community and payment

There is no membership fee and no payment gateway in the community portal's current direction. Do not add checkout, billing, or payment processing unless Andrew changes this decision. Say joining is free; do not imply registered-charity or tax-deductible status unless verified.

## 8. Governance and traceability

- Keep lasting product decisions in DECISIONS.md.
- Record material requests and implementation handoffs in COMMUNICATION_LOG.md.
- Link implementation changes to GitHub commits and pull requests.
- Mark planned features as planned; do not describe them as live.
- Review changes to child participation, accounts, data collection, moderation, or payments against these principles before implementation.

## 9. Privacy reference

Malaysia's Personal Data Protection Regulations 2013 state that consent for processing the personal data of a person under 18 is to be obtained from a parent, guardian, or person with parental responsibility. The Personal Data Protection Department's Data Protection by Design Guideline also calls for valid guardian consent and data minimisation for under-18 data. Review current requirements and the final privacy notice with qualified Malaysian privacy counsel before collecting children's data.

- [Personal Data Protection Regulations 2013 (official JPDP PDF)](https://www.pdp.gov.my/ppdpv1/wp-content/uploads/2024/07/Peraturan-peraturan-Perlindungan-Data-Peribadi.pdf)
- [Data Protection by Design Guideline (official JPDP PDF)](https://www.pdp.gov.my/wp-content/uploads/2026/04/Data-Protection-By-Design-Guideline-DpbD.pdf)
