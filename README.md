# Aziz Ali

**AI-native engineer in Stockholm.** I build agentic systems and ship them: a live iOS app, a client site in production, and tools I use every day. [azizali.dev](https://azizali.dev) · [LinkedIn](https://www.linkedin.com/in/aziz-ali-138a241b3/)

## Selected work

**[Kap](https://apps.apple.com/us/app/kap-reklamblad-erbjudanden/id6792043652)** (live on the iOS App Store). Swedish grocery-deals app with a Gemini function-calling agent that may cite only deals a tool returned in that request. 15 flyer-source adapters feed it; a 13-check golden-query eval suite runs after each ingest. Expo/React Native, Bun + Hono, SQLite.

**career-hq** (private). A governed agentic pipeline for my own job search: it reads public ATS APIs under a throttle, triages postings with an LLM scored against labelled jobs, and agents draft. Every state change goes through one CLI into an append-only log with its actor, and hooks refuse protected edits. It never applies; I do. 88 Vitest spec files plus 40 Bun test files.

**FlowStaff** ([flowstaff.se](https://flowstaff.se)). Site and prospects CRM for a real staffing client. Next.js, Supabase, strict Content-Security-Policy with HSTS preload, AI drafts that wait for a person before anything is sent.

**sleep-watch** (private, being prepared for release). Camera sleep monitor that runs fully local: adaptive frame-differencing motion detection plus Silero VAD for speech, SQLite storage, self-contained HTML night reports. Python, OpenCV, onnxruntime. 136 pytest tests.

## How I work

Agents draft, evals gate, and a human approves whatever cannot be undone. I keep agent write paths narrow and logged, and put an eval or test in front of the behaviour I rely on (Kap's golden queries, career-hq's triage scorecard). Claude Code is my daily tool, with hooks and skills I wrote around it.

## Also here

[quitter](https://github.com/zizo2001/quitter): quit several Mac apps at once from the menu bar.
