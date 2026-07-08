<div align="center">

<!-- Capsule Render Banner -->
<img src="https://capsule-render.vercel.app/api?type=rect&color=161730,291642,42309f,5f189a,2e38a5&height=170&section=header&text=Tyler%20Cox%20%E2%80%A2%20Software%20Engineer&fontColor=f4f4f5&fontSize=45&fontAlignY=40&animation=fadeIn&customColorList=purple,indigo,blue" alt="Tyler Cox Banner"/>

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=24&pause=1000&vCenter=true&width=740&lines=MacroMesh%3A+AI+Nutrition+App+I%E2%80%99m+Shipping+and+Maintaining;Ohio+State+CSE+Student+%7C+Intern%2FNew+Grad+Roles;SwiftUI+%7C+Next.js+%7C+TypeScript+%7C+OpenAI+API;Frontend+%2B+Backend+%2B+Mobile+%2B+Deployment" alt="Typing SVG" />

<br/>

<!-- Badges -->
<p align="center">
  <a href="https://www.linkedin.com/in/tyler-cox-53b886406" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-Tyler%20Cox-0077b5?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=23212f" alt="LinkedIn"/></a>
  <a href="mailto:Tyler.cox66@yahoo.com" target="_blank"><img src="https://img.shields.io/badge/Email-Tyler.cox66%40yahoo.com-6a5acd?style=for-the-badge&logo=gmail&logoColor=white&labelColor=23212f" alt="Email"/></a>
  <a href="https://tyler-portfolio-site.vercel.app" target="_blank"><img src="https://img.shields.io/badge/Portfolio-tyler--portfolio--site-6532b1?style=for-the-badge&logo=vercel&logoColor=white&labelColor=23212f" alt="Portfolio"/></a>
  <a href="https://github.com/TyCodes101" target="_blank"><img src="https://img.shields.io/badge/GitHub-TyCodes101-24292f?style=for-the-badge&logo=github&logoColor=white&labelColor=23212f" alt="GitHub"/></a>
</p>
<p align="center">
  <img src="https://komarev.com/ghpvc/?username=TyCodes101&label=Profile+Views&color=4c2885&style=flat"/>
</p>
<p align="center">
  <img src="https://img.shields.io/static/v1?label=Based%20In&message=Columbus%2C%20Ohio&color=3e23c1&style=flat-square&logo=googlemaps" />
</p>

</div>

---

## About Me

Hi, I’m Tyler. I study Computer Science & Engineering at The Ohio State University, and most of my time outside class goes into building and maintaining MacroMesh—an AI nutrition app that I’m actively shipping and improving.

I like projects where the details matter: turning messy real-world input into reliable data, building interfaces that feel fast and clear on mobile, and keeping a system stable as features grow. I’m most comfortable working across the stack (SwiftUI + Next.js + TypeScript + Postgres) and I’m looking for software engineering internship and new grad opportunities.

---

## MacroMesh (centerpiece)

<p align="center">
  <a href="https://github.com/TyCodes101/calorie-compass" target="_blank"><img src="https://img.shields.io/badge/Repo-calorie--compass-6a5acd?style=for-the-badge&logo=github&logoColor=white&labelColor=23212f" alt="MacroMesh Repo"/></a>
  <img src="https://img.shields.io/badge/SwiftUI-iOS-4c2885?style=for-the-badge&logo=swift&logoColor=white&labelColor=23212f" alt="SwiftUI"/>
  <img src="https://img.shields.io/badge/Next.js-API-111827?style=for-the-badge&logo=nextdotjs&logoColor=white&labelColor=23212f" alt="Next.js"/>
  <img src="https://img.shields.io/badge/TypeScript-App%20%2B%20API-2b6cb0?style=for-the-badge&logo=typescript&logoColor=white&labelColor=23212f" alt="TypeScript"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/OpenAI-Meal%20Parsing-3b82f6?style=for-the-badge&logo=openai&logoColor=white&labelColor=23212f" alt="OpenAI"/>
  <img src="https://img.shields.io/badge/Postgres-Data-2563eb?style=for-the-badge&logo=postgresql&logoColor=white&labelColor=23212f" alt="Postgres"/>
  <img src="https://img.shields.io/badge/Prisma-ORM-4338ca?style=for-the-badge&logo=prisma&logoColor=white&labelColor=23212f" alt="Prisma"/>
  <img src="https://img.shields.io/badge/Vercel-Deploy-1f2937?style=for-the-badge&logo=vercel&logoColor=white&labelColor=23212f" alt="Vercel"/>
  <img src="https://img.shields.io/badge/Codemagic-CI%2FCD-4f46e5?style=for-the-badge&logo=codemagic&logoColor=white&labelColor=23212f" alt="Codemagic"/>
  <img src="https://img.shields.io/badge/TestFlight-iOS%20Beta-312e81?style=for-the-badge&logo=apple&logoColor=white&labelColor=23212f" alt="TestFlight"/>
</p>

MacroMesh began as a personal “I wish this existed” project. Meal logging should be fast, but it also has to be trustworthy—especially when an AI is involved. So the core product idea is simple: let the user write food naturally, use AI to help interpret it, and then make every important detail reviewable before it’s saved.

<table width="100%" style="font-size:15px">
  <tr>
    <td width="24%"><b>What it solves</b></td>
    <td>Turns natural-language meal descriptions into structured, reviewable macro logs—without forcing a long, rigid form flow.</td>
  </tr>
  <tr>
    <td><b>Trust model</b></td>
    <td>Nothing is auto-saved. AI output becomes a draft; the user confirms/edits before it becomes history.</td>
  </tr>
  <tr>
    <td><b>Key system</b></td>
    <td>A food resolver pipeline that handles ambiguity, source confidence, and fallback behavior when a match is weak.</td>
  </tr>
  <tr>
    <td><b>Shipping workflow</b></td>
    <td>Vercel for the web/API surface, Codemagic + fastlane/TestFlight for iOS builds.</td>
  </tr>
</table>

### Architecture (high level)

```mermaid
flowchart LR
 A["iOS App<br/>SwiftUI"] -->|"Auth + API calls"| B["Next.js API<br/>TypeScript"]
 C["Web App<br/>Next.js"] -->|"Meal logging"| B
 B --> D["OpenAI<br/>Intent + meal parsing"]
 B --> E["Food Resolver<br/>Deterministic + provider layers"]
 E --> F[("Postgres<br/>Prisma")]
 B --> F
 B --> A
 B --> C
```

<details>
<summary><strong>Engineering notes (the part I spend most of my time on)</strong></summary>
<br/>

<table width="100%" style="font-size:15px">
  <tr>
    <td width="24%"><b>AI meal parsing</b></td>
    <td>The AI is used for intent + structure. Nutrition trust still comes from the resolver/provider pipeline, and every draft stays editable.</td>
  </tr>
  <tr>
    <td><b>Resolver design</b></td>
    <td>Resolver prefers deterministic matches and saved corrections when possible, then uses model assistance when needed. It also produces “this is uncertain” states instead of pretending it knows.</td>
  </tr>
  <tr>
    <td><b>Review-before-save UX</b></td>
    <td>The UI treats the AI output like a suggestion, not a fact. This is the biggest difference between a “cool AI demo” and something people can actually keep using.</td>
  </tr>
  <tr>
    <td><b>Reliability work</b></td>
    <td>When OpenAI is unavailable (or keys aren’t set locally), the app has deterministic fallbacks so the core loop still works during development and testing.</td>
  </tr>
  <tr>
    <td><b>Testing</b></td>
    <td>Guardrails include unit tests and a multi-turn assistant QA suite to catch regressions in logging accuracy and correction behavior.</td>
  </tr>
</table>

<b>Docs worth skimming (if you like seeing the thinking):</b>
<br/>
- https://github.com/TyCodes101/calorie-compass/blob/main/docs/openai-food-intelligence.md
- https://github.com/TyCodes101/calorie-compass/blob/main/docs/food-logging-production-hardening-audit.md
- https://github.com/TyCodes101/calorie-compass/blob/main/docs/NUTRITION_INTELLIGENCE_AUDIT.md

</details>

### Development timeline (recent)

<table>
  <tr><td width="18%"><b>July 2026</b></td><td>Improved the resolver flow for ambiguous meal descriptions and expanded automated test coverage around failure modes.</td></tr>
  <tr><td><b>June 2026</b></td><td>Tightened the TestFlight pipeline and reduced friction in the release loop (Codemagic + fastlane handoff).</td></tr>
  <tr><td><b>May 2026</b></td><td>Iterated on the macro dashboard and onboarding to make the core loop faster on mobile.</td></tr>
</table>

### Roadmap

<table>
  <tr><td width="18%"><b>Now</b></td><td>Resolver accuracy, review UX, and reliability under API/provider failure.</td></tr>
  <tr><td><b>Next</b></td><td>Expand food matching coverage, improve caching, and add more confidence/attribution in the UI.</td></tr>
  <tr><td><b>Later</b></td><td>Build out barcode/OCR flows further (kept behind review-first drafts, not auto-save).</td></tr>
</table>

---

## Other Projects

<details>
<summary><strong>Stride Step Tracker</strong></summary>
A React Native/Expo app for tracking steps and calorie balance with straightforward daily feedback. I built it with local-first persistence and real empty states, so the UI behaves honestly when there’s no data.

https://github.com/TyCodes101/stride-step-tracker
</details>

<details>
<summary><strong>CPU Scheduler Visualizer</strong></summary>
A React/Vite visualizer for FCFS, SJF, Priority, and Round Robin scheduling. The goal was to turn OS scheduling into something you can play with and understand quickly.

https://tycodes101.github.io/cpu-scheduler-visualizer/
https://github.com/TyCodes101/cpu-scheduler-visualizer
</details>

---

## Toolset (what shows up in my repos)

<table width="100%" style="font-size:15px">
  <tr><td width="24%"><b>Languages</b></td><td>TypeScript, Swift, JavaScript, HTML/CSS</td></tr>
  <tr><td><b>Frameworks</b></td><td>SwiftUI, Next.js, React, Expo</td></tr>
  <tr><td><b>AI</b></td><td>OpenAI API (structured outputs + contracts, meal/intent parsing)</td></tr>
  <tr><td><b>Data</b></td><td>Postgres, Prisma</td></tr>
  <tr><td><b>Deployment</b></td><td>Vercel, GitHub Pages</td></tr>
  <tr><td><b>CI/CD</b></td><td>Codemagic, GitHub Actions</td></tr>
  <tr><td><b>Testing</b></td><td>Vitest, Jest (project-dependent)</td></tr>
</table>

---

## How I Build (practical)

I try to build software people can actually keep using. I keep interfaces simple, test before shipping, and iterate based on what breaks or confuses users. I care a lot about maintainable code because I like revisiting a project months later and still being able to move fast.

---

## Quick Links

<p align="center">
  <a href="https://tyler-portfolio-site.vercel.app" target="_blank">Portfolio</a> •
  <a href="https://www.linkedin.com/in/tyler-cox-53b886406" target="_blank">LinkedIn</a> •
  <a href="mailto:Tyler.cox66@yahoo.com" target="_blank">Email</a> •
  <a href="https://github.com/TyCodes101" target="_blank">GitHub</a>
</p>

---

## GitHub Analytics (verified providers)

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=TyCodes101&theme=tokyonight" alt="GitHub Stats" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=TyCodes101&theme=tokyonight" alt="Top Languages" />
</p>
<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=TyCodes101&theme=react-dark&hide_border=true" alt="Activity Graph"/>
</p>

---

<div align="center">
<i>Build for real people. Keep it simple. Test before shipping. Learn from every release.</i>
<br/><br/>
<img src="https://capsule-render.vercel.app/api?section=footer&type=waving&color=161730,291642,42309f,5f189a,2e38a5&height=90" alt="Capsule Render Footer"/>
</div>
