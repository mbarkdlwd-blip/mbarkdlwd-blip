# Portfolio Projects

Only projects whose source code is in the GitHub account were assessed. **Two credible portfolio projects exist today, not five.** The Flutter emergency-rooms app and the NUSelle website were listed in your brief but are not in the account; they can be added once their code is pushed.

## Presentation order

### 1. Nyalatna AI Registration & Admissions Platform ⭐ flagship

**Repository:** `mbarkdlwd-blip/nyalatna-ai-agent` (private)

**One-line pitch:** An admissions, payments and finance system for a training center in Sudan, with an AI assistant that registers applicants over web chat, WhatsApp and Messenger in Arabic.

**Problem.** Course registration, fee collection and finance were manual, which made batch capacity and payment records hard to keep consistent, while most applicants ask questions over chat in Sudanese Arabic.

**Stack (verified):** C#, .NET 10, ASP.NET Core Minimal APIs, EF Core 10, PostgreSQL, OpenAI .NET SDK, QuestPDF, React 19, TypeScript, Vite, xUnit, Vitest, Docker, GitHub Actions.

**Implemented features**
- Applicants, courses, batches with capacity, atomic registrations with status rules.
- Payments with installments, verification by a second staff member (segregation of duties), reversal.
- Funds, revenues, expenses and a PDF financial report in Arabic.
- AI registration assistant with guardrails and cost controls.
- WhatsApp, Messenger and Facebook-comment integration through a signed Meta webhook.
- Role-based access (15 policies), audit log, soft delete, rate limiting, password reset.

**Evidence**
- 101 backend integration test methods on real PostgreSQL; passing in GitHub Actions.
- 42 frontend unit tests passing; typecheck and production build passing; 0 npm vulnerabilities.
- Five design and operations documents (configuration, database, deployment, security, testing).

**Key technical challenges**
- Preventing over-booking and duplicate numbering under concurrent registrations.
- Letting an LLM drive registration without letting it bypass business rules or confirm payments.
- Enforcing financial segregation of duties in both the API and the UI.
- Arabic/RTL interface and Arabic PDF generation.

**Status:** Active development, functional. Meta channels not yet verified with live credentials.

**Presentation advice.** The repository is private. Recruiters cannot see it, so either:
- make it public after confirming credential rotation and that no real applicant data is in the repo (none was found), or
- keep it private and feature it on the profile README with screenshots and a short write-up, offering access on request.

**Portfolio suitability:** Excellent. It demonstrates backend engineering, database design, testing discipline, security thinking and applied AI, all in one real-world project.

### 2. C++ Programming & Data Structures Coursework

**Repository:** `mbarkdlwd-blip/202510537_DSA_MubarakDawoodAbdalla` (public)

**One-line pitch:** Seven C++ console programs from university coursework, from pointers to a multi-file, class-based library management system.

**Stack:** C++17, standard library (`vector`, `fstream`, `sstream`, `iomanip`).

**Highlights:** library management system with a `LibraryBook` class, overdue detection and fines; ATM with PIN lockout and transaction history; file-backed student CRUD.

**Evidence:** six programs compile in CI; each was run with scripted input during the audit.

**Status:** Coursework. One program (07) is incomplete because its header is missing.

**Portfolio suitability:** Good as a learning record showing C++ fundamentals and OOP. Feature it below the flagship, not as a headline project.

## Not yet on GitHub

| Project | From your brief | What is needed |
|---|---|---|
| South Darfur Emergency Rooms app | Flutter, Dart, Firebase | Push the code, keeping `google-services.json` and API keys out of the repo |
| NUSelle website | HTML, CSS, JavaScript, Netlify | Push the site; add the Netlify URL as the repository homepage |

Once pushed, both would add mobile and front-end range to the portfolio. They would then need the same audit.

## Not for the portfolio

`202510537_DSA_MubarakDawoodAbdall`: empty duplicate; recommended for deletion.
