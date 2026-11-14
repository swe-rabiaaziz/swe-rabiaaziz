<div align="center">

<img src="assets/hero.svg" alt="Rabia Aziz — Flutter Developer & Mobile App Engineer" width="100%"/>

<br/>

<a href="https://swe-rabia-aziz.vercel.app/"><img src="https://img.shields.io/badge/PORTFOLIO-FAFAFA?style=for-the-badge&logo=vercel&logoColor=09090B" alt="Portfolio"/></a>
<a href="https://www.linkedin.com/in/swe-rabiaaziz/"><img src="https://img.shields.io/badge/LINKEDIN-18181B?style=for-the-badge&labelColor=18181B&color=18181B&logoColor=FAFAFA" alt="LinkedIn"/></a>
<a href="https://www.tiktok.com/@swe.rabiaaziz"><img src="https://img.shields.io/badge/TIKTOK_·_5.4K-18181B?style=for-the-badge&logo=tiktok&logoColor=FAFAFA" alt="TikTok"/></a>
<a href="mailto:swe.rabiaaziz@gmail.com"><img src="https://img.shields.io/badge/EMAIL-18181B?style=for-the-badge&logo=gmail&logoColor=FAFAFA" alt="Email"/></a>
<a href="https://calendly.com/swe-rabiaaziz/30min"><img src="https://img.shields.io/badge/BOOK_A_CALL-FAFAFA?style=for-the-badge&logo=calendly&logoColor=09090B" alt="Book a call"/></a>

</div>

<br/>

<img src="assets/divider.svg" width="100%" alt=""/>

## 01 · What I do

I take products from a rough idea to a polished, store-ready app. Here is what I deliver to founders and engineering teams:

<img src="assets/services.svg" width="100%" alt="Production MVPs, Figma to Flutter, AI and Voice integration, Backend and Cloud architecture, Code audits and refactoring"/>

<br/>

<img src="assets/divider.svg" width="100%" alt=""/>

## 02 · Shipped to stores

Four apps live on Google Play, built, designed and released end to end.

<table>
<tr>
<td width="50%" valign="top">

#### ◆ CivicCoach
**AI US Citizenship Test 2026**

An AI oral mock-interview simulator with all 128 official questions, spaced repetition and an offline-first Drift / SQLite database.

<a href="https://play.google.com/store/search?q=CivicCoach%20AI%20US%20Citizenship%20Test&c=apps"><img src="https://img.shields.io/badge/GOOGLE_PLAY-FAFAFA?style=for-the-badge&logo=googleplay&logoColor=09090B" alt="CivicCoach on Google Play"/></a>

</td>
<td width="50%" valign="top">

#### ◆ ZenPeace
**Pomodoro & Mindful Flow**

A minimalist focus timer with ambient audio soundscapes, reactive `fl_chart` analytics and clean Provider-driven state flow.

<a href="https://play.google.com/store/search?q=ZenPeace%20Pomodoro&c=apps"><img src="https://img.shields.io/badge/GOOGLE_PLAY-FAFAFA?style=for-the-badge&logo=googleplay&logoColor=09090B" alt="ZenPeace on Google Play"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### ◆ Zemen
**Ethiopian Calendar**

A 13-month Ge'ez calendar with a dual Gregorian / Ethiopian date converter and a sunrise clock.

<a href="https://play.google.com/store/search?q=Zemen%20Ethiopian%20Calendar&c=apps"><img src="https://img.shields.io/badge/GOOGLE_PLAY-FAFAFA?style=for-the-badge&logo=googleplay&logoColor=09090B" alt="Zemen on Google Play"/></a>

</td>
<td width="50%" valign="top">

#### ◆ Health Tracker
**Vitals & BP Monitor**

Blood-pressure tracking and pulse trends with private, on-device SQLite storage.

<a href="https://play.google.com/store/search?q=Health%20Tracker%20Vitals%20BP%20Monitor&c=apps"><img src="https://img.shields.io/badge/GOOGLE_PLAY-FAFAFA?style=for-the-badge&logo=googleplay&logoColor=09090B" alt="Health Tracker on Google Play"/></a>

</td>
</tr>
</table>

<img src="assets/divider.svg" width="100%" alt=""/>

## 03 · How I ship

Anyone can make a screen look good in a demo. What matters is whether it still feels right on a mid-range phone, six months and forty features later.

### The performance standard

<img src="assets/performance.svg" width="100%" alt="60/120fps frame budget, Impeller testing, widget rebuild optimisation"/>

### Folder architecture

A modular, feature-first structure with a strict dependency rule: `presentation → domain ← data`.

```text
lib/
├── core/                  # theme, router, DI, constants, error handling, utils
├── features/
│   └── <feature>/
│       ├── data/          # remote + local data sources, models, repository impls
│       ├── domain/        # entities, repository contracts, use cases
│       └── presentation/  # pages, widgets, BLoC / Provider
└── main.dart
```

### State management rulebook

| Reach for | When | Why |
| :-- | :-- | :-- |
| **BLoC / Cubit** | Complex async flows: auth, streamed LLM responses, multi-step sessions, anything event-driven | Explicit events and states make flows predictable, testable and easy to trace |
| **Provider** | Reactive UI state: timers, theme, toggles, lightweight view state | Minimal boilerplate and scoped rebuilds for state that stays close to the UI |

### Offline-first principle

The local database is the source of truth. The UI never waits on the network.

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#111113','primaryTextColor':'#fafafa','primaryBorderColor':'#52525b','lineColor':'#a1a1aa','secondaryColor':'#18181b','tertiaryColor':'#09090b','fontFamily':'monospace'}}}%%
flowchart LR
  UI["UI · Flutter widgets"] <--> SM["BLoC / Provider"]
  SM <--> REPO["Repository"]
  REPO <--> LOCAL[("Local DB<br/>Drift · SQLite · Hive")]
  REPO <-. background sync .-> CLOUD[("Cloud<br/>Supabase · Firebase")]
```

<img src="assets/divider.svg" width="100%" alt=""/>

## 04 · Tech stack & ecosystem

<img src="assets/marquee.svg" width="100%" alt="Tech stack marquee"/>

<br/>

<table>
<tr>
<td width="220"><b>Mobile & Languages</b></td>
<td>
<img src="https://img.shields.io/badge/Dart-18181B?style=for-the-badge&logo=dart&logoColor=FAFAFA" alt="Dart"/>
<img src="https://img.shields.io/badge/Flutter-18181B?style=for-the-badge&logo=flutter&logoColor=FAFAFA" alt="Flutter"/>
<img src="https://img.shields.io/badge/Android-18181B?style=for-the-badge&logo=android&logoColor=FAFAFA" alt="Android"/>
<img src="https://img.shields.io/badge/iOS-18181B?style=for-the-badge&logo=apple&logoColor=FAFAFA" alt="iOS"/>
<img src="https://img.shields.io/badge/Web-18181B?style=for-the-badge&logo=googlechrome&logoColor=FAFAFA" alt="Web"/>
</td>
</tr>
<tr>
<td><b>State Management</b></td>
<td>
<img src="https://img.shields.io/badge/BLoC_/_Cubit-18181B?style=for-the-badge&logoColor=FAFAFA" alt="BLoC / Cubit"/>
<img src="https://img.shields.io/badge/Provider-18181B?style=for-the-badge&logoColor=FAFAFA" alt="Provider"/>
</td>
</tr>
<tr>
<td><b>Cloud & Databases</b></td>
<td>
<img src="https://img.shields.io/badge/Supabase-18181B?style=for-the-badge&logo=supabase&logoColor=FAFAFA" alt="Supabase"/>
<img src="https://img.shields.io/badge/Firebase-18181B?style=for-the-badge&logo=firebase&logoColor=FAFAFA" alt="Firebase"/>
<img src="https://img.shields.io/badge/PostgreSQL-18181B?style=for-the-badge&logo=postgresql&logoColor=FAFAFA" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/SQLite-18181B?style=for-the-badge&logo=sqlite&logoColor=FAFAFA" alt="SQLite"/>
<img src="https://img.shields.io/badge/Drift-18181B?style=for-the-badge&logoColor=FAFAFA" alt="Drift"/>
<img src="https://img.shields.io/badge/Hive-18181B?style=for-the-badge&logoColor=FAFAFA" alt="Hive"/>
</td>
</tr>
<tr>
<td><b>AI & Hardware</b></td>
<td>
<img src="https://img.shields.io/badge/Speech--to--Text-18181B?style=for-the-badge&logo=googleassistant&logoColor=FAFAFA" alt="Speech-to-Text"/>
<img src="https://img.shields.io/badge/Audio_Players-18181B?style=for-the-badge&logoColor=FAFAFA" alt="Audio Players"/>
<img src="https://img.shields.io/badge/Google_ML_Kit-18181B?style=for-the-badge&logo=google&logoColor=FAFAFA" alt="Google ML Kit"/>
</td>
</tr>
<tr>
<td><b>Tooling</b></td>
<td>
<img src="https://img.shields.io/badge/Git-18181B?style=for-the-badge&logo=git&logoColor=FAFAFA" alt="Git"/>
<img src="https://img.shields.io/badge/GitHub_Actions-18181B?style=for-the-badge&logo=githubactions&logoColor=FAFAFA" alt="GitHub Actions"/>
<img src="https://img.shields.io/badge/Figma-18181B?style=for-the-badge&logo=figma&logoColor=FAFAFA" alt="Figma"/>
<img src="https://img.shields.io/badge/Android_Studio-18181B?style=for-the-badge&logo=androidstudio&logoColor=FAFAFA" alt="Android Studio"/>
<img src="https://img.shields.io/badge/VS_Code-18181B?style=for-the-badge&logo=visualstudiocode&logoColor=FAFAFA" alt="VS Code"/>
</td>
</tr>
</table>

<img src="assets/divider.svg" width="100%" alt=""/>

<!--
=====================================================================
05 · ENDORSEMENTS  (hidden until you add REAL quotes)
Replace the placeholders below with genuine words from the people
named, get their OK, then delete the "<!--" line above and the
"-->" line at the bottom of this block to publish the section.
=====================================================================

## 05 · What collaborators say

<table>
<tr>
<td width="33%" valign="top">

> "PASTE A REAL 1–2 SENTENCE QUOTE HERE."

**Muhammad Uzair**<br/>
<sub>Role / relationship</sub>

</td>
<td width="33%" valign="top">

> "PASTE A REAL 1–2 SENTENCE QUOTE HERE."

**Afaq Zahir**<br/>
<sub>Role / relationship</sub>

</td>
<td width="33%" valign="top">

> "PASTE A REAL 1–2 SENTENCE QUOTE HERE."

**Past project lead**<br/>
<sub>Role / relationship</sub>

</td>
</tr>
</table>

<img src="assets/divider.svg" width="100%" alt=""/>
-->

## 05 · Stats & activity

<div align="center">

<img height="190" src="https://github-readme-stats.vercel.app/api?username=swe-rabiaaziz&show_icons=true&hide_border=false&bg_color=09090B&title_color=FAFAFA&text_color=A1A1AA&icon_color=FAFAFA&border_color=27272A&ring_color=FAFAFA&border_radius=16&include_all_commits=true&count_private=true" alt="GitHub stats"/>
<img height="190" src="https://github-readme-stats.vercel.app/api/top-langs/?username=swe-rabiaaziz&layout=compact&langs_count=6&bg_color=09090B&title_color=FAFAFA&text_color=A1A1AA&border_color=27272A&border_radius=16" alt="Top languages"/>

<img src="https://streak-stats.demolab.com?user=swe-rabiaaziz&background=09090B&ring=FAFAFA&fire=FAFAFA&currStreakLabel=FAFAFA&currStreakNum=FAFAFA&sideLabels=A1A1AA&sideNums=FAFAFA&dates=71717A&stroke=27272A&border=27272A&border_radius=16" alt="GitHub streak"/>

<br/><br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/swe-rabiaaziz/swe-rabiaaziz/output/github-snake-dark.svg"/>
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/swe-rabiaaziz/swe-rabiaaziz/output/github-snake.svg" width="100%"/>
</picture>

</div>

<br/>

<img src="assets/divider.svg" width="100%" alt=""/>

## 06 · Let's work together

<img src="assets/cta.svg" width="100%" alt="Let's build something that ships. Open to full-time remote roles and freelance builds."/>

<div align="center">

<br/>

<a href="https://calendly.com/swe-rabiaaziz/30min"><img src="https://img.shields.io/badge/BOOK_A_30_MIN_CALL-FAFAFA?style=for-the-badge&logo=calendly&logoColor=09090B" alt="Book a call"/></a>
<a href="mailto:swe.rabiaaziz@gmail.com"><img src="https://img.shields.io/badge/swe.rabiaaziz@gmail.com-18181B?style=for-the-badge&logo=gmail&logoColor=FAFAFA" alt="Email me"/></a>
<a href="https://swe-rabia-aziz.vercel.app/"><img src="https://img.shields.io/badge/VIEW_PORTFOLIO-18181B?style=for-the-badge&logo=vercel&logoColor=FAFAFA" alt="Portfolio"/></a>

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:09090b,100:3f3f46&height=120&section=footer" width="100%" alt=""/>

</div>
