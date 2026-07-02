# Gulf ECG Diary — MVP prototype

A bilingual (English / Arabic, with RTL) **clinician-reviewed single-lead ECG diary** prototype for the Gulf region, built as a single self-contained `index.html` for GitHub Pages.

> **Working brand only.** Not affiliated with, endorsed by, or owned by AliveCor / Kardia. KardiaMobile / Apple Watch ECG are named only as example consumer devices.

## ⚠️ What this is

This is a **static, clickable prototype** — the right thing for a "test it out" link. GitHub Pages serves static files only, so:

- **Payments are mocked** (Stripe test-card UI, no real charge).
- **Uploads are mocked** — files never leave your browser; only metadata is stored.
- **All state lives in this browser** via `localStorage`. Clearing site data resets everything.

A production build would use the stack in the spec (Next.js + Supabase + Stripe + Resend on Vercel).

## What it demonstrates

- Bilingual EN/AR with proper RTL layout and a calm, evidence-first clinical design.
- A **Learn** library of patient education (palpitations, triggers, the attention loop, 4–6 breathing, vagal techniques, sleep, alcohol, weight/movement, omega-3 caution, single-lead ECG devices, HRV, ectopics/AF/SVT, the CAST lesson) — adapted from the owner's OpenPalp programme, with UK-specific terms replaced by Gulf-appropriate wording.
- Eligibility + **9-question red-flag screen** that routes emergencies to `NOT_ELIGIBLE_EMERGENCY_ADVICE`.
- **Payment slider SAR 1–149 with no default / no suggested amount** (button stays disabled until you choose).
- 7-day diary with a **20-upload-per-episode** cap and a platform **1,000-uploads-per-month** cap.
- Patient dashboard, ECG upload with priority-flagging for concerning symptoms.
- **Clinician/admin dashboard**: metrics, review queue + filters, per-ECG classification & signal-quality, consolidated report builder, sign/issue, escalate, physiologist-QA assignment.
- Patient report view + print-to-PDF + WhatsApp share.

## Try it

1. Open the site → **Start ECG diary review** → complete the screen (answer **No** to all red-flags to stay eligible).
2. Choose any amount on the slider → pay (test mode) → upload a file or two.
3. Open **Clinician** in the header → sign in (no password) → **Load demo cases** to populate the queue → open a case, classify ECGs, build & sign a report.
4. Toggle **العربية** in the header to see the full RTL Arabic experience.

## Run locally

Just open `index.html` in a browser — no build step.

---

*Arabic copy is MSA with Gulf-friendly wording and should be reviewed by a native Arabic medical reviewer before launch. Educational content is general information, not personal medical advice. Final legal wording must be reviewed before launch.*
