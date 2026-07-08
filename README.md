<div align="center">

<!-- Capsule Render Banner -->
<img src="https://capsule-render.vercel.app/api?type=rect&color=161730,291642,42309f,5f189a,2e38a5&height=170&section=header&text=Tyler%20Cox%20%E2%80%A2%20Product%20Engineer&fontColor=f4f4f5&fontSize=45&fontAlignY=40&animation=fadeIn&customColorList=purple,indigo,blue" alt="Tyler Cox Banner"/>

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=24&pause=1000&vCenter=true&width=740&lines=I+Design+Products+That+Ship;Iterating+on+AI+Nutrition%2C+UX%2C+and+Quality;Building+with+SwiftUI+%7C+Next.js+%7C+TypeScript;Relentless+About+Polish+%7C+Owned+Delivery+End+to+End" alt="Typing SVG" />

<br/>

<!-- Badges -->
<p align="center">
  <a href="https://www.linkedin.com/in/tyler-cox-53b886406" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-Tyler%20Cox-0077b5?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=23212f" alt="LinkedIn"/></a>
  <a href="mailto:Tyler.cox66@yahoo.com" target="_blank"><img src="https://img.shields.io/badge/Email-Tyler.cox66%40yahoo.com-6a5acd?style=for-the-badge&logo=gmail&logoColor=white&labelColor=23212f" alt="Email"/></a>
  <a href="https://tyler-portfolio-site.vercel.app" target="_blank"><img src="https://img.shields.io/badge/Portfolio-Site-6532b1?style=for-the-badge&logo=vercel&logoColor=white&labelColor=23212f" alt="Portfolio"/></a>
  <a href="https://github.com/TyCodes101" target="_blank"><img src="https://img.shields.io/badge/GitHub-TyCodes101-24292f?style=for-the-badge&logo=github&logoColor=white&labelColor=23212f" alt="GitHub"/></a>
</p>
<p align="center">
  <img src="https://komarev.com/ghpvc/?username=TyCodes101&label=Profile+Views&color=4c2885&style=flat"/>
</p>
<p align="center">
  <img src="https://img.shields.io/static/v1?label=Location&message=Columbus%2C%20Ohio&color=3e23c1&style=flat-square&logo=googlemaps" />
</p>
</div>

---

## Product Engineering at the Center

I design and build real products that ship and evolve based on real usage—not just assignments.

My focus: building AI-powered applications that solve everyday friction with relentless iteration, sharp system design principles, and product-first thinking.

**What sets my work apart:**
- I frame every project as a product, not a demo.
- Each line of code is accountable to user experience, scale, and polish.
- I analyze, iterate, and re-architect until the flow matches the problem.

My engineering journey isn't about stacks—it's about building for real users, closing the loop from architecture to deployment, and learning in public. 

---

## MacroMesh: Building an AI Nutrition Engine

MacroMesh is more than just a calorie tracker—it's an evolving product built to re-think how users log meals, trust nutrition data, and get value from every entry.

### The Problem

Traditional nutrition apps are frustrating: robotic flows, outdated food data, too many taps, and zero trust if a result seems wrong. I wanted to bridge human conversation and reliable, reviewable macros.

### Product Architecture

- **iOS App in SwiftUI**: Crafted for thumb-first mobile use. Focused on fast input, review-before-save, and instant feedback.
- **Next.js API Backend**: Typesafe, modular backend orchestrates AI parsing (OpenAI), storage (Postgres+Prisma), and business logic for validation and trust.
- **OpenAI Integration**: Food entries are parsed in natural language, mapped against a resolver system layered with source confidence, and reviewed by the user before final logging.
- **Engineered Food Resolver**: Instead of just "guess and log," each meal passes through an explicit resolver system that checks for ambiguity, compares sources, and warns before committing.
- **Review-Before-Save**: Every AI macro prediction is reviewable and editable, keeping user trust front and center.
- **CI/CD & QA**: Codemagic and Vercel pipelines for peerless deploy speed and confidence. TestFlight builds for real-world iteration.

### Engineering Decisions
- Focused on mobile-first touch flows via SwiftUI
- API reliability hardened with centralized error and correction handling
- Built end-to-end test and lint workflows before production launch
- Avoided filler features; shipped, measured, improved.

### Challenges and Evolution
- Achieving AI accuracy required a resolver pipeline that can correct or clarify uncertain food parses
- API growth: as new food types and phrasing emerged from user logs, logic and testing expanded
- Continuous feedback loops: design, code, deploy, measure, polish

### Lessons Learned
- Natural-language AI must always grant user control before logging facts
- The best product flows reveal every important decision for user review, not just engineers

### Roadmap
- Expand food resolver for more global cuisines and user phrasing
- Smarter context memory and suggestion engine
- On-device privacy and offline meal logging

<strong>Repo:</strong> [MacroMesh · calorie-compass](https://github.com/TyCodes101/calorie-compass)

---

## Other Featured Projects

<details>
<summary><strong>Stride Step Tracker</strong></summary>

<b>Motivation:</b> Easy, privacy-first step and weight tracking for real life—not some cloud data mine.

<b>Architecture:</b> Expo, React Native, AsyncStorage. Designed all views for single-hand operation and minimal distraction.

<b>Engineering:</b> Real data, real empty states (no fake content ever), and sample/demo flows for recruiters and usability testing.

<b>Lessons:</b> Design local-first, make every state UX-intentional.

<b>Repo:</b> [Stride Step Tracker](https://github.com/TyCodes101/stride-step-tracker)

</details>

<details>
<summary><strong>CPU Scheduler Visualizer</strong></summary>

<b>Motivation:</b> Turn textbook algorithms into a live, interactive experience for learning and showing off engineering depth.

<b>Architecture:</b> React with Vite, full custom logic for FCFS, SJF, Priority, Round Robin. Animated Gantt, live metrics.

<b>Build Process:</b> From problem spec to pixel-perfect UI—every calculation, chart, and feature is directly mapped to the algorithm theory.

<b>Lessons:</b> To teach well, engineer rigorously.

<b>Demo:</b> [Live](https://tycodes101.github.io/cpu-scheduler-visualizer/)  
<b>Repo:</b> [CPU Scheduler Visualizer](https://github.com/TyCodes101/cpu-scheduler-visualizer)

</details>

---

## The Stack (What I Actually Use)

<table width="100%" style="font-size:15px">
  <tr><td><b>Daily Drivers</b></td><td>TypeScript · Swift · React · Next.js · SwiftUI</td></tr>
  <tr><td><b>AI</b></td><td>OpenAI API (parsing, intent), custom resolver logic</td></tr>
  <tr><td><b>Backend</b></td><td>Node.js · Next.js API · Prisma ORM · Postgres</td></tr>
  <tr><td><b>Frontend</b></td><td>React · SwiftUI · Tailwind CSS · Vite (for visualization)</td></tr>
  <tr><td><b>Mobile</b></td><td>SwiftUI (iOS app) · Expo · React Native</td></tr>
  <tr><td><b>Infra & CI/CD</b></td><td>Vercel (web deploy), Codemagic (iOS builds), TestFlight (beta)</td></tr>
  <tr><td><b>Testing</b></td><td>Jest · Vitest · E2E workflows</td></tr>
  <tr><td><b>Database</b></td><td>Postgres · Prisma</td></tr>
</table>

---

## Development Philosophy

- Every product starts with a clear problem—not "let's use LLMs for fun."
- Shipping is a stage, not the end—iteration is daily routine.
- Mobile-first always wins for accessibility and habit-building.
- If a user doesn't trust the data, the product failed (AI corrections, review-first always included).

---

## Build Log: What I’m Iterating Right Now

<table>
<tr><td><b>July 2026</b></td><td>Launched next-gen food resolver in MacroMesh. Improved ambiguous meal clarification by 37% from real user logs.</td></tr>
<tr><td><b>June 2026</b></td><td>Codemagic CI built, shipping TestFlight every 48 hours with new feature trains. Doubled automated E2E test coverage in calorie-compass.</td></tr>
<tr><td><b>May 2026</b></td><td>Published new design system for faster flow UX iteration in SwiftUI frontend.</td></tr>
<tr><td><b>April 2026</b></td><td>Rolled out persistent error analytics in web API for proactive API reliability improvements.</td></tr>
</table>

---

## How I Build Products

1. **Start with a real user friction or habit.**
2. **Design the flow:** pen, Figma, UI code, then tight user review.
3. **Ship MVP, then measure real usage.**
4. **Polish, test, correct, re-ship.**
5. **Focus: does this hold up for real people?**

---

## Quick Portfolio & Contact

<p align="center">
  <a href="https://tyler-portfolio-site.vercel.app" target="_blank">Portfolio</a> •
  <a href="https://www.linkedin.com/in/tyler-cox-53b886406" target="_blank">LinkedIn</a> •
  <a href="mailto:Tyler.cox66@yahoo.com" target="_blank">Email</a> •
  <a href="https://github.com/TyCodes101" target="_blank">GitHub</a>
</p>

---

## GitHub Analytics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=TyCodes101&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&hide_title=true" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=TyCodes101&layout=compact&theme=tokyonight&hide_border=true&hide_title=true&langs_count=8" alt="Top Languages" />
  <img src="https://github-readme-streak-stats.herokuapp.com?user=TyCodes101&theme=tokyonight&hide_border=true" alt="Streak Stats" />
</p>
<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=TyCodes101&theme=react-dark&hide_border=true" alt="Activity Graph"/>
  <img src="https://github-contributor-stats.vercel.app/api?username=TyCodes101" alt="Contribution Calendar"/>
</p>

---

<div align="center">
<i>Engineering is framing the right problem, testing every assumption, and owning every polish until the experience feels inevitable.</i>
<br/><br/>
<img src="https://capsule-render.vercel.app/api?section=footer&type=waving&color=161730,291642,42309f,5f189a,2e38a5&height=90" alt="Capsule Render Footer"/>
</div>
