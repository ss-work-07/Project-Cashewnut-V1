# CentAI — AI Interview Practice Suite

**Live demo: [project-cashewnut.vercel.app](https://project-cashewnut.vercel.app/)**

> This repo is a showcase only. The source code is in a private repository and is not published here. Try the live deployment above to see the product.

CentAI helps candidates get ready for interviews in **11 job profiles** across engineering, AI & data, product and go-to-market. It has three tools.

## Tools

### 🎙️ Interviewer
A mock interview in several rounds, each of which must be passed to unlock the next. It is grounded in your resume and in what the market expects for the role.
- Type your answers or speak them (speech-to-text transcription)
- Follow-up questions that adapt to what you said
- The AI interviewer can read each question aloud, with mute and replay controls
- Ends with a **readiness scorecard** that shows your strengths, your priority gaps and a short practice plan

### 📄 Resume Optimizer
- An ATS-style readiness score
- Rewrite suggestions for each bullet point
- Detection of missing keywords, checked against the target role's skill rubric

### ❓ Question Generator
- A bank of practice questions sorted by category and tagged by difficulty
- Built from the role's rubric and your resume

## Supported Roles

| Engineering | AI & Data | Product & Business |
|---|---|---|
| Backend Engineer | AI Builder | Product Manager |
| Frontend Engineer | AI Engineer | Consultant |
| Full-Stack Engineer | Data Scientist | Sales Professional |
| Forward Deployed Engineer | ML Engineer | |

## Tech Stack

- **Framework:** Next.js 16 (App Router), React, TypeScript
- **AI providers:** Google Gemini (question generation and scorecards) and Groq (Whisper speech-to-text and text-to-speech), with automatic choice between them
- **Validation:** Zod
- **Resume parsing:** PDF text extraction on the server, within set limits
- **Testing:** Vitest (unit tests and evals), Playwright (end-to-end user journeys)
- **Hosting:** Vercel

## Design Highlights

- **Privacy first:** resume PDFs and voice recordings are processed in memory and never stored. Interview state stays in the user's browser session.
- **API keys stay on the server:** every AI call goes through server routes, and no key is sent to the browser.
- **Demo mode:** the full interview flow works even without an AI provider, so the product is always available to try.
- **Data-driven roles:** role rubrics, levels, rounds and company types are defined as data, so new roles can be added without changing the UI.

## Screenshots

_Coming soon._

---

© 2026. All rights reserved. Source code available on request.
