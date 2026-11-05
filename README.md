<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=220&section=header&text=Saathwik%20Bhamidipaty&fontSize=52&fontAlignY=40&fontColor=ffffff&animation=fadeIn&desc=Software%20Engineer%20in%20the%20Making%20%E2%80%94%20Builder%20at%20Heart&descAlignY=62&descSize=16&descColor=a78bfa" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=20&pause=1200&color=A78BFA&center=true&vCenter=true&random=false&width=650&lines=Hey+there%2C+I'm+Saathwik+%F0%9F%91%8B;CS+%40+University+of+Illinois+Chicago;I+build+things+from+scratch+%E2%80%94+end+to+end;C%2B%2B+%7C+Java+%7C+Swift+%7C+Python;Currently+seeking+SWE+Internships+%F0%9F%9A%80)](https://git.io/typing-svg)

<p>
  <a href="https://www.linkedin.com/in/saathwikbhamidipaty">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:bhamidipatysaathwik@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://github.com/BhamSaath">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <img src="https://komarev.com/ghpvc/?username=BhamSaath&label=Profile+Views&color=7c3aed&style=for-the-badge"/>
</p>

</div>

---

## `$ whoami`

```yaml
name        : Saathwik Bhamidipaty
location    : Chicago, IL 🏙️
education   : B.S. Computer Science — University of Illinois Chicago
              Expected Graduation: Winter 2028
focus       : Software Engineering Internships
core_skills : [C++, Java, Swift, Python, SQLite, pybind11, Gemini API, Git]
learning    : [YAML, Linux, GitHub Agentic AI]
languages   : [English, Telugu, Hindi]
fun_fact    : "Built a full cricket analytics engine in C++ that queries 23,000+ matches — yes, entirely from scratch."
```

---

## ⚡ Right Now

<table>
<tr>
<td width="50%">

**🎓 Coursework in Progress**
- C Programming & Software Tools
- Data Structures & Algorithms (CS 251)
- Assembly & Machine Organization (CS 261)
- Discrete Math for Computer Science
- Engineering Probability & Statistics
- Linear Algebra
- Multivariable & Vector Calculus

</td>
<td width="50%">

**🔭 Currently Working On**
- 🏏 Cricket Analytics & AI Matchup Engine — shipped, expanding
- 📜 GitHub Agentic AI Certification
- 🛠️ Expanding my C++ & Java project portfolio
- 🔍 Actively hunting SWE internships
- 🏏 Recently wrapped as Captain of Stevenson Cricket Club

</td>
</tr>
</table>

---

## 🛠️ Tech Stack

<div align="center">

**Languages**

[![Skills](https://skillicons.dev/icons?i=cpp,java,swift,python,git,linux,github&theme=dark&perline=7)](https://skillicons.dev)

**Concepts & Tools**

| Area | What I Know |
|---|---|
| 🧱 Architecture | OOP, Multi-class Inheritance, Enumerations, Subclassing |
| ⚡ Performance | C++/Python FFI via pybind11, shared library compilation |
| 🔐 Security | Bcrypt hashing, password ≠ storage separation |
| 💾 Data | SQLite indexing, JSON persistence (nlohmann/json) |
| 🤖 AI & Backend | Gemini API, structured LLM prompting, REST APIs |
| 🔗 Integration | API Integration, Error Analysis & Debugging |
| 📐 Math | Multivariable Calculus, Linear Algebra |

</div>

---

## 🏗️ Featured Projects

### 🏏 Cricket Analytics & AI Matchup Engine — *Hero Project*
> *C++ aggregation engine + Python orchestration + Gemini API — querying 23,000+ real match records.*

[![Cricket Stats Scraper](https://github-readme-stats.vercel.app/api/pin/?username=BhamSaath&repo=Cricket-Stats-Scraper&theme=midnight-purple&border_color=7c3aed&title_color=a78bfa&icon_color=a78bfa&cache_seconds=86400)](https://github.com/BhamSaath/Cricket-Stats-Scraper)

The core problem was speed. Parsing 23,000 raw JSON files per query took 2–3 minutes. The solution: index everything into SQLite once, write the aggregation layer in C++, and expose it to Python via a pybind11 shared library. Queries now run in milliseconds.

```
  User Input (player / venue)
            │
            ▼
  ┌─────────────────────────┐
  │   Python Orchestration  │
  │   Routes query mode     │
  │   (PVP or PVG)          │
  └────────────┬────────────┘
               │  pybind11 call
               ▼
  ┌─────────────────────────┐
  │   C++ Aggregation Layer │
  │   PVP.cpp / PVG.cpp     │
  │   Queries SQLite        │
  │   Computes per-format   │
  │   stats per delivery    │
  └────────────┬────────────┘
               │  AggregateStats struct
               ▼
  ┌─────────────────────────┐
  │   SQLite Database       │
  │   23,000+ matches       │
  │   indexed by player,    │
  │   venue, match type     │
  └────────────┬────────────┘
               │
               ▼
  ┌─────────────────────────┐
  │   Gemini API            │
  │   Stats → prompt        │
  │   Natural language out  │
  └────────────┬────────────┘
               ▼
     Terminal output + summary
```

| What | How |
|---|---|
| ⚡ Performance | SQLite indexing dropped query time from 2–3 min → milliseconds |
| 🔗 C++/Python bridge | pybind11 shared library (`statsPVP.so`) |
| 🤖 AI layer | Gemini only sees computed stats — no hallucinated figures |
| 📊 Query modes | PVP (head-to-head) and PVG (player at venue), all 3 formats |
| 🛠️ Process | Solo end-to-end — architecture → C++ → Python → shipped |

**[→ Explore the Repository](https://github.com/BhamSaath/Cricket-Stats-Scraper)**

---

### 🏏 Cricket Workload Tracker & Player Management System

[![Cricket Workload Tracker](https://github-readme-stats.vercel.app/api/pin/?username=BhamSaath&repo=cricket-workload-tracker&theme=midnight-purple&border_color=7c3aed&title_color=a78bfa&icon_color=a78bfa&cache_seconds=86400)](https://github.com/BhamSaath/cricket-workload-tracker)

Terminal-based C++ application for coaches and players to manage rosters, training plans, sessions, and injury logs. Multi-class OOP architecture with Bcrypt auth and full JSON persistence across sessions.

| What | How |
|---|---|
| 🔐 Auth | Bcrypt — password verification stays isolated from user data |
| 💾 Persistence | nlohmann/json — full session history survives across logins |
| 🧩 Design | 3+ core classes, enumerations, role-specific subclasses |
| 🎭 Roles | Dual-mode: Coach view & Player view |

**[→ Explore the Repository](https://github.com/BhamSaath/cricket-workload-tracker)**

---

## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats-git-master-me-0de5.vercel.app/api?username=BhamSaath&show_icons=true&theme=midnight-purple&border_color=7c3aed&title_color=a78bfa&icon_color=a78bfa&hide_border=false&rank_icon=github&cache_seconds=86400" height="170" alt="GitHub Stats" />
  <img src="https://github-readme-stats-git-master-me-0de5.vercel.app/api/top-langs/?username=BhamSaath&theme=midnight-purple&border_color=7c3aed&title_color=a78bfa&layout=compact&langs_count=6&cache_seconds=86400" height="170" alt="Top Languages" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=BhamSaath&theme=midnight-purple&border=7c3aed&ring=a78bfa&fire=f59e0b&currStreakLabel=a78bfa&sideLabels=a78bfa&dates=a78bfa" width="520" alt="GitHub Streak" />
</div>

<div align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=BhamSaath&theme=github_dark" width="720" alt="Profile Details" />
</div>

---

## 🏆 Certifications

<div align="center">

| Badge | Certification | Platform | Status |
|:---:|---|---|:---:|
| 🎖️ | **GitHub Foundations** | LinkedIn Learning | ✅ Earned |

</div>

---

## 🏏 Leadership Beyond the Terminal

<div align="center">

```
Stevenson Cricket Club — Leader & Captain  |  Aug 2024 – May 2026
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  Active Members    ██████████████████████  2× growth
  Practice Sessions ██████████████████████  1 → 3 per week (200% ↑)
  Team Standards    ██████████████████████  Built from scratch
```

Overhauled recruitment, tripled practice frequency, and established team communication standards that accelerated player development across the board. Same skills, different domain.

</div>

---

## 📬 Let's Talk

<div align="center">

**I'm actively looking for Software Engineering Internship opportunities.**
If you're building something interesting — I want to help build it.

[![LinkedIn](https://img.shields.io/badge/Connect%20on%20LinkedIn-%230A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/saathwikbhamidipaty)
[![Email Me](https://img.shields.io/badge/Email%20Me-%23EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:bhamidipatysaathwik@gmail.com)
[![View My Code](https://img.shields.io/badge/View%20My%20Code-%23181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/BhamSaath)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=120&section=footer" width="100%"/>

</div>
