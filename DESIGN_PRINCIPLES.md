# AI Generation Community — Design Principles

**Status:** Founder-approved product direction; implementation requirements remain gated until built and reviewed.  
**Owner:** Andrew Tan  
**Last updated:** 2026-11-20 (Malaysia time)

This document guides the portal's content, user experience, and future membership features. It does not claim planned safeguards or account features already exist.

## 1. Purpose and audience

AI Generation Community is a free, non-commercial community initiative for families, educators, learners, makers, and partners in Malaysia to learn about AI, create useful projects, and share what they learn.

The first page must explain the value to parents and guardians before asking a family to join. Children participate with a trusted adult's guidance. The site must not position a child as an independent sign-up target.

## 2. Parent-first trust

Every child-facing invitation should explain what families can learn or make, what the parent or guardian does, what data is collected and why, how sharing and contact work, and how reporting, moderation, and deletion are handled.

Future child participation must default to adult-led registration and parent oversight, no public child profile, no unsolicited direct messaging, and parent review before a child's work is made public. Community rules, reporting, and an operating moderation process must be ready before member interaction or user-generated content is enabled. Collect the minimum information needed; prefer a nickname and age band over full name, exact birth date, school, phone, or address.

These are implementation requirements, not claims about current functionality. Do not promise moderation or safety controls until they are live and staffed.

## 3. First-page experience

The homepage should make this journey clear:

1. Understand the community's purpose and value.
2. Recognize that a parent, guardian, educator, or adult is the joining adult.
3. Understand the first activities and participation expectations.
4. Review community guidelines and privacy information.
5. Register or express interest only through a path that is actually implemented.

Use one clear adult-facing action, such as **Join as a parent, educator or adult member**, plus a secondary **Explore together** action. Explain the **Learn · Make · Share** model.

### Homepage copy draft

| English | 中文 | Bahasa Melayu |
|---|---|---|
| **Building tomorrow's AI generation — together.** A community for families, educators and curious minds to explore AI through guided learning, hands-on projects and responsible sharing. | **一起培养面向未来的 AI 新一代。** 为家庭、教育工作者和好奇的学习者打造一个社区，通过引导式学习、动手项目和负责任的分享，一起认识与探索 AI。 | **Bersama membina generasi AI masa hadapan.** Komuniti untuk keluarga, pendidik dan mereka yang ingin tahu meneroka AI melalui pembelajaran berpandu, projek praktikal dan perkongsian yang bertanggungjawab. |
| **Join as a parent, educator or adult member** · **Explore AI together** | **家长、教育工作者或成人会员加入** · **和孩子一起探索 AI** | **Sertai sebagai ibu bapa, pendidik atau ahli dewasa** · **Teroka AI bersama** |
| **For children to explore—with a trusted adult by their side.** Parents or guardians help choose activities, guide participation and decide what a child shares. | **孩子可以探索，家长在身边引导。** 家长或监护人陪伴孩子选择活动、参与探索，并决定哪些作品适合分享。 | **Ruang untuk anak meneroka dengan bimbingan orang dewasa yang dipercayai.** Ibu bapa atau penjaga membantu memilih aktiviti, membimbing penyertaan dan menentukan perkara yang boleh dikongsi. |
| **Learn · Make · Share** | **学习 · 创造 · 分享** | **Belajar · Cipta · Kongsi** |
| **Free to join · No payment required** | **免费加入 · 无需付款** | **Pendaftaran percuma · Tiada bayaran diperlukan** |

## 4. Language parity

English, Simplified Chinese, and Bahasa Melayu are first-class experiences. Core navigation, calls to action, parent guidance, privacy notices, and community rules must be available in all three languages. Switching languages must not interrupt the visitor's journey or silently reset their selection.

## 5. Visual direction

Build a bold, editorial, Malaysia-rooted experience: an immersive local hero image, confident typography, warm cream and forest-green accents, and vivid cards for family activities, young creator projects, workshops, and upcoming events. Make it feel active through real activities, community work, and stories rather than decorative AI graphics alone. Show only verified events, projects, partners, testimonials, and impact; label planned programmes as coming soon. Keep the family guidance visible, accessible, and mobile-friendly. Use concept art only when clearly identified, and do not imply unbuilt features or protections. Official logo, colors, and brand assets remain subject to founder approval.

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
