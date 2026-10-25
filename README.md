<div align="center">

# Hi, I'm Gianfranco Larocca 👋

### Full-Stack Developer · PHP / Laravel · Vue.js · Flutter

<a href="https://github.com/GianfrancoLarocca">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1000&color=FF2D20&center=true&vCenter=true&width=600&lines=Full-Stack+Developer+%40+AGF+Energy;Laravel+%2B+Vue.js+in+production+since+2024;Flutter+%2B+Laravel+on+my+side+projects;Open+to+new+opportunities+%E2%80%94+relocation+included" alt="Typing SVG" />
</a>

<p>
  <a href="https://www.linkedin.com/in/gianfrancolarocca4j"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:gianfrancolarocca4j@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://leetcode.com/u/Giancotsu/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
</p>

<img src="https://img.shields.io/badge/📍_Bari,_Italy-555555?style=flat-square" alt="Bari, Italy" />
<img src="https://img.shields.io/badge/✅_Open_to_work-on--site_·_hybrid_·_remote_·_relocation-2ea44f?style=flat-square" alt="Open to work" />

</div>

---

## 👨‍💻 About me

I'm a **full-stack developer** focused on **PHP/Laravel** backends and **Vue.js** frontends.
At **AGF Energy** I build and maintain the company's internal management software: new features driven by business needs, refactoring of existing modules, REST APIs and MySQL data handling.

On my own I go further: I ship cross-platform apps with **Flutter**, and I keep growing on **Java/Spring Boot** and **Angular/TypeScript**.
I care about **clean, maintainable code**, solid architectures and automated tests.

```yaml
role:        Full-Stack Developer @ AGF Energy S.p.A. (Aug 2024 – present)
daily_stack: [PHP, Laravel, JavaScript, Vue.js, MySQL]
also_using:  [Dart, Flutter, Java, Spring Boot, TypeScript, Angular, Docker]
location:    Bari, Italy
open_to:     [on-site, hybrid, remote, relocation]
```

---

## 🛠️ Tech stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=php,laravel,js,vue,html,css,bootstrap&perline=7" alt="Web stack" /><br/>
  <img src="https://skillicons.dev/icons?i=dart,flutter,java,spring,ts,angular&perline=7" alt="Mobile and Java stack" /><br/>
  <img src="https://skillicons.dev/icons?i=mysql,postgres,sqlite,docker,git,github,githubactions,linux&perline=8" alt="Data and tools" />
</p>

| Area | Technologies |
|---|---|
| **Backend** | PHP · Laravel (Eloquent, Sanctum, Scheduler) · REST APIs · Java · Spring Boot |
| **Frontend** | Vue.js · JavaScript · TypeScript · Angular · HTML5 · CSS3 |
| **Mobile** | Dart · Flutter (Riverpod, go_router, drift) |
| **Database** | MySQL · PostgreSQL · SQLite |
| **DevOps & tools** | Git · GitHub Actions (CI) · Docker · Linux |

---

## 💼 Experience

### Full-Stack Developer · AGF Energy S.p.A.
📅 *August 2024 – present* · 📍 *Bari*

- Develop and maintain the company's **internal management applications** (Laravel + Vue.js)
- Ship **new features** driven by business requirements
- **Refactor** and maintain existing pages and modules
- Design and integrate **REST APIs** and handle data on **MySQL**
- Automate internal processes (data import/export, workflows, cron jobs)
- Performance monitoring and application debugging

**Tech:** PHP · Laravel · JavaScript · Vue.js · MySQL

---

## ⭐ Featured project

### 💰 CashLogs: cross-platform personal finance app

> Budget and expense tracker for **Android, iOS and Web (PWA)**, with its own **Laravel REST API** and **MySQL** backend.
> **Status:** feature-complete, getting ready for the store release · 🔒 *private repository (commercial project), happy to walk through it in an interview*

<p>
  <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter" />
  <img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white" alt="Dart" />
  <img src="https://img.shields.io/badge/Riverpod-00B4AB?style=flat-square" alt="Riverpod" />
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/PHP_8.3-777BB4?style=flat-square&logo=php&logoColor=white" alt="PHP 8.3" />
  <img src="https://img.shields.io/badge/MySQL_8-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL 8" />
  <img src="https://img.shields.io/badge/SQLite_(drift)-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />
</p>

**What it does**
- Multiple accounts and currencies, with **daily exchange rates** fetched by a scheduled job
- Categories and subcategories, recurring transactions, transfers, **loans with installments**, bill splitting
- **Budgets** with per-category limits and overspending alerts, **savings goals**
- Statistics: pie charts, trends, calendar heatmap, period history
- File and photo attachments, spreadsheet import, data export, backups, deep links to add transactions
- Biometric **app lock**, local notifications, Italian and English localization

**How it's built**
- 📴 **Offline-first sync:** local SQLite cache (drift), an outbox queue, client-generated UUIDs, delta sync (`GET/POST /api/sync`), soft deletes and *last-write-wins* conflict resolution. The server is the source of truth.
- 💶 **Correct money handling:** amounts stored as integers in minor units plus an ISO 4217 currency code. No floats, ever.
- 🔐 **API security:** Laravel Sanctum tokens, FormRequest validation, Policies so every user sees only their own data, API Resources, plus the account-deletion and privacy pages the app stores require
- 🧱 **Feature-based architecture:** `features/<feature>/{data,domain,presentation}` in Flutter, with Riverpod for state and go_router for navigation
- ✅ **Quality gates:** about **1,380 automated tests** (Flutter unit and widget tests, Laravel feature tests), CI on GitHub Actions against a **real MySQL 8**, Laravel Pint, and `flutter analyze` with zero warnings
- 🤖 **AI-assisted workflow:** I designed an autonomous development pipeline with Claude Code: a written functional spec, a task plan, a verification script and a CI gate. I review every branch through a pull request before merging.

---

## 📊 GitHub & LeetCode

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=GianfrancoLarocca&show_icons=true&include_all_commits=true&hide_border=true&bg_color=00000000&title_color=FF2D20&icon_color=FF2D20&text_color=8b949e" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=GianfrancoLarocca&layout=compact&hide_border=true&bg_color=00000000&title_color=FF2D20&text_color=8b949e" alt="Top languages" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=GianfrancoLarocca&hide_border=true&background=00000000&ring=FF2D20&fire=FF2D20&currStreakLabel=FF2D20&sideLabels=8b949e&dates=8b949e&currStreakNum=8b949e&sideNums=8b949e" alt="GitHub streak" />
</p>

<p align="center">
  <a href="https://leetcode.com/u/Giancotsu/">
    <img src="https://leetcard.jacoblin.cool/Giancotsu?theme=dark&font=Fira%20Code&ext=heatmap" alt="LeetCode stats" />
  </a>
</p>

---

## 🎓 Education & certifications

**Technical High School Diploma, Computer Science (Diploma Tecnico Tecnologico, Settore Informatico)**
Istituto Tecnico Tecnologico e Scientifico *Guglielmo Marconi* · 2017

**Cisco Networking Academy**
- CCNA Discovery: Networking for Home and Small Businesses
- CCNA Routing and Switching: Introduction to Networks
- CCNA: Internet of Everything

Since graduating I've kept learning **on my own**: web development, backend engineering, database design, and now mobile with Flutter.

---

## 🏍️ Outside the code

Motorbikes and **chess** ♟️: I like strategy, on the board as much as in software architecture.

---

<div align="center">

### 📬 Let's talk

I'm open to new opportunities, **including relocating to another city**.

<a href="https://www.linkedin.com/in/gianfrancolarocca4j"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:gianfrancolarocca4j@gmail.com"><img src="https://img.shields.io/badge/gianfrancolarocca4j@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

</div>
