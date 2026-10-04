<div align="center">

# `<Jad Said />`

### Senior software engineer & founder · Beirut

**Complex systems. Clear decisions. *Shipped products.***

[![Portfolio](https://img.shields.io/badge/portfolio-jadsaidd.me-F37021?style=flat-square&logo=googlechrome&logoColor=white)](https://www.jadsaidd.me)
[![WhatsApp](https://img.shields.io/badge/whatsapp-+961_71_817_030-25D366?style=flat-square&logo=whatsapp&logoColor=white)](https://wa.me/96171817030)
[![LinkedIn](https://img.shields.io/badge/linkedin-jad_said-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jad-said-3b3626237/)
[![X](https://img.shields.io/badge/x-@jadsaidd-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/jadsaidd)
[![Email](https://img.shields.io/badge/email-jadsaidd@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:jadsaidd@gmail.com)

</div>

```console
jad@software ~ % whoami
Jad Said · computer engineer (LIU) · shipping since 2020

jad@software ~ % cat now.txt
Founding Engineer   @ Taste and Telemetry
Owner & Architect   @ JSS Technology
Founder             @ Mentorly · CLLYNK

jad@software ~ % ai --status
✓ using AI
✕ used by AI
```

---

## How I build

- **Correctness lives in the database.** Exclusion constraints stop double bookings, unique keys stop a seat selling twice, and transactions re-check limits, so the rule holds even when two requests land at once.
- **Every table starts locked.** Access is fail-closed by default, and a test or a build check proves the public key can read nothing sensitive.
- **Webhooks are the source of truth for money.** The payment provider settles it; a daily sweep catches anything a webhook missed.
- **Realtime without flooding.** Throttle by time *and* distance, keep presence in Redis with a TTL, and push only the deltas.
- **Ship, then measure in production.** Crashlytics, audits and real data decide what gets fixed next, not guesses.

---

## Stack

| Layer | Tools |
|---|---|
| **Mobile** | Flutter · Dart · React Native |
| **Web** | Next.js · React · TypeScript · Tailwind CSS · Payload CMS |
| **Backend** | Node.js · Express · GraphQL · Django · Spring Boot · Supabase |
| **Data & realtime** | PostgreSQL · PostGIS · Prisma · Redis · BullMQ · Celery · Socket.IO · Qdrant |
| **AI** | OpenAI · Anthropic · LangChain · vector search · intent detection |
| **Payments & integrations** | Stripe · Shopify (Liquid) · Klaviyo · Twilio · Resend · Google Maps · Firebase |
| **Delivery** | Docker · GitHub Actions · Vercel · Playwright · Vitest · Jest |

<p align="left">
  <img src="https://skillicons.dev/icons?i=flutter,dart,react,nextjs,ts,nodejs,express,graphql,django,spring,postgres,prisma,redis,supabase,firebase,docker,githubactions,vercel,tailwind&perline=10" alt="Stack icons" />
</p>

---

## Selected systems

| Project | Problem | What I did |
|---|---|---|
| **[Jeye](https://jeye.app)**<br><sub>Food delivery · tech lead</sub> | Drivers must keep broadcasting location while backgrounded on patchy networks. | Socket.IO location stream throttled by time and distance. Last position in Redis (60s TTL) and presence on a separate 90s heartbeat. Fees from real driving distance and elevation, priced per region with PostGIS. Order acceptance runs in a strict transaction. **First commit to launch in ~4 months.** |
| **[Winterland](https://www.winterland-alain.ae/en)**<br><sub>Event ticketing · architect</sub> | Thousands of people booking the same seats the moment tickets open. | Venue modelled down to zone, section, row and seat. A per-show unique seat constraint plus transactional bookings, and one Flutter app for buying tickets and scanning them at the gate. **5,000+ users in the first 24 hours.** |
| **Kilow**<br><sub>Digital health · backend</sub> | A fragile backend under constantly changing business rules. | Re-architected it: one job system on BullMQ, a real-time support CRM over Socket.IO, pluggable payment strategies, and a WhatsApp assistant with vector-backed intent detection (Qdrant) and per-conversation memory. |
| **[Minaka](https://www.minaka.app)**<br><sub>Venue OS · founding engineer</sub> | A vibe-coded app leaking data and losing payments. | Closed a row-level-security hole the database advisor missed, moved to a single fail-closed permission check, fixed six unauthenticated endpoints and split platform billing from venue payments on Stripe. |
| **[The Garage KC](https://thegaragekc.com)**<br><sub>Members club · solo</sub> | Applications, invoicing, a member portal and a staff console, fast. | Three apps on one Supabase source of truth: overlapping bookings are rejected by a Postgres exclusion constraint, invoicing settles by webhook, and emails go out through an outbox. **Built in two weeks.** |
| **[Nextgrab](https://www.nextgrab.co)**<br><sub>Food rescue · project lead</sub> | An AI-built prototype that broke under real users. | Rebuilt it in Flutter and Firebase: zoom- and distance-based map loading, pickup confirmed by QR, OTA code push, Crashlytics, and payment reconciliation shared by the admin and vendor dashboards. |
| **[PSA](https://system.psa-scout.com)**<br><sub>Scouts platform · volunteer</sub> | Daily operations for non-technical leaders, in Arabic. | Arabic-first, right-to-left dashboard, an offline-first Flutter app with an encrypted check-in queue, and digital ID cards with QR codes. **3,000 members use it daily.** |

<sub>More in the full write-ups at <a href="https://www.jadsaidd.me/work">jadsaidd.me/work</a>.</sub>

---

## Experience

| When | Role |
|---|---|
| 2026 – now | **Founding Engineer** · Taste and Telemetry |
| 2025 – 2026 | **Senior Engineer** · Nextgrab |
| 2025 – 2026 | **Senior Software Engineer** · Kilow |
| 2024 – 2025 | **CTO** · 3E Tech |
| 2023 – 2025 | **Senior Software Engineer** · Talodon |
| 2021 – 2023 | **Mobile Application Developer** · Megabee |
| 2021 – 2023 | **Frontend Developer** · Horizon Web-Solutions |

**Founded:** [JSS Technology](https://www.jss.technology) (owner & software architect) · [Mentorly](https://mentorly.tech) (technical oversight for founders) · CLLYNK (coming soon)

---

<div align="center">

**Building something hard?** WhatsApp is the fastest way to reach me.

[jadsaidd.me](https://www.jadsaidd.me) · [JSS Technology](https://github.com/JSS-Technology) · [Mentorly](https://github.com/mentorly-tech)

</div>
