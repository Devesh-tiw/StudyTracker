<div align="center">

# ⬡ StudyCore

### **The Ultimate Engineering Study Tracker**

*A sleek, dark-themed, fully client-side study management dashboard built for engineering students who want to take control of their academic life.*

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)](https://www.chartjs.org/)

[![License: MIT](https://img.shields.io/badge/License-MIT-00e5ff.svg?style=for-the-badge)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-7c3aed.svg?style=for-the-badge)](CONTRIBUTING.md)
[![Maintenance](https://img.shields.io/badge/Maintained-Yes-10b981.svg?style=for-the-badge)](https://github.com/yourusername/studycore)

<br/>

[**🚀 Live Demo**](https://yourusername.github.io/studycore) · [**🐛 Report Bug**](https://github.com/yourusername/studycore/issues) · [**💡 Request Feature**](https://github.com/yourusername/studycore/issues)

<br/>

<img src="https://raw.githubusercontent.com/yourusername/studycore/main/screenshots/dashboard.png" alt="StudyCore Dashboard" width="90%"/>

</div>

---

## 📋 Table of Contents

- [About](#-about)
- [Features](#-features)
- [Screenshots](#-screenshots)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Usage Guide](#-usage-guide)
- [Project Structure](#-project-structure)
- [Keyboard Shortcuts](#-keyboard-shortcuts)
- [Data & Privacy](#-data--privacy)
- [Browser Support](#-browser-support)
- [Contributing](#-contributing)
- [Roadmap](#-roadmap)
- [License](#-license)
- [Acknowledgments](#-acknowledgments)

---

## 🎯 About

**StudyCore** is a comprehensive, zero-dependency study management dashboard designed specifically for **engineering students**. It provides a beautiful, distraction-free interface to plan daily tasks, set weekly goals, manage monthly schedules, track subjects, and analyze your study performance — all from a single HTML file.

### ❓ Why StudyCore?

| Problem | StudyCore Solution |
|---|---|
| 🔴 Scattered study plans across notebooks & apps | ✅ One unified dashboard for everything |
| 🔴 No visibility into study patterns | ✅ Rich charts & analytics show your progress |
| 🔴 Cloud-dependent tools need accounts & internet | ✅ 100% offline, no account needed |
| 🔴 Complex tools with steep learning curves | ✅ Clean UI, zero setup, instant start |
| 🔴 Privacy concerns with cloud storage | ✅ All data stays on YOUR device |

---

## ✨ Features

### 📊 Dashboard
> Your command center — see everything at a glance
- **Real-time stats**: Today's tasks, completion count, weekly goals, total subjects
- **Weekly progress chart**: Bar chart showing tasks created vs completed over the last 7 days
- **Subject distribution**: Doughnut chart breaking down tasks by subject
- **Quick Add**: Instantly add tasks without leaving the dashboard

### ◈ Day Tasks
> Plan, track, and conquer your daily workload
- Create tasks with **title, subject, priority, date, and notes**
- **Three priority levels**: 🔴 High, 🟡 Medium, 🟢 Low
- **Completion tracking** with visual progress bar
- **Priority distribution** doughnut chart
- Filter tasks by any date
- One-click toggle to mark tasks done/undone

### ◉ Week Goals
> Set ambitious weekly targets and track your progress
- Create goals with **custom targets** (e.g., "Complete 10 DSA problems")
- **+1 / -1 controls** for quick progress updates
- **Weekly calendar view** showing tasks per day
- **Horizontal bar chart** comparing targets vs progress
- Color-coded goals for visual organization

### ▦ Month Planner
> Bird's-eye view of your entire month
- **Interactive calendar** with day-click planning
- Add plans with **custom tags**: Study, Exam, Assignment, Lab, Project, Revision
- **Color-coded dots** indicate days with plans or tasks
- **Monthly task distribution** bar chart
- Navigate between months with Previous/Next controls
- Chronological plan list with tag badges

### ◫ Subjects
> Organize your engineering curriculum
- Add subjects with **name, code, and custom color**
- Per-subject **completion percentage** with progress bars
- **7-day activity sparkline** for each subject
- Visual cards with hover animations
- Subjects auto-populate in all task dropdowns

### ◆ Skills & Extras
> Track what makes you unique beyond academics
- Track skills with **custom icons** (💻🔬🧮🎨🎵 and more)
- **Four skill levels**: Beginner → Intermediate → Advanced → Expert
- **Categories**: Technical Skill, Favorite Subject, Hobby, Language, Tool/Framework
- **Radar chart** visualizing skill distribution (3+ skills)
- **Progress bars** showing mastery level per skill

### ◬ Reports & Analytics
> Deep dive into your study patterns
- **4 report tabs**: Overview, By Subject, Daily Trend, Priority Analysis
- **Overview**: Total tasks, completed count, completion rate, day streak
- **By Subject**: Per-subject cards with stats and mini charts
- **Daily Trend**: 14-day bar chart of task activity
- **Priority Analysis**: Breakdown by priority with completion rates

### 🛡️ Data Management
- **Auto-save** to localStorage — data persists across sessions
- **Reset All Data** button with confirmation prompt
- **Delete confirmations** for important actions
- **Zero data leaves your device** — complete privacy

---

## 📸 Screenshots

<div align="center">

| Dashboard | Day Tasks |
|---|---|
| ![Dashboard](screenshots/dashboard.png) | ![Day Tasks](screenshots/daytasks.png) |

| Week Goals | Month Planner |
|---|---|
| ![Week Goals](screenshots/weekgoals.png) | ![Month Planner](screenshots/monthplan.png) |

| Subjects | Skills & Extras |
|---|---|
| ![Subjects](screenshots/subjects.png) | ![Skills](screenshots/skills.png) |

| Reports - Overview | Reports - Priority |
|---|---|
| ![Reports](screenshots/reports.png) | ![Priority](screenshots/priority.png) |

</div>

---

## 🛠 Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Semantic structure & layout |
| **CSS3** | Custom properties, Grid, Flexbox, animations |
| **Vanilla JavaScript** | All logic, state management, DOM manipulation |
| **Chart.js 4.4.1** | Bar, Line, Doughnut, Radar charts |
| **Google Fonts** | Syne (headings) + Space Mono (data) |
| **localStorage API** | Client-side data persistence |

### 🏗 Architecture
========================================================================================
                                     STUDYCORE APP                                      
========================================================================================
[  SIDEBAR (NAV) AREA  ] | [                    MAIN CONTENT REGION                    ]
------------------------+---------------------------------------------------------------
                         | [ PAGE HEADER ] --> [ ⬡ Dash ]
                         |--------------------------------------------------------------

                         | [ ◈ Tasks ] | [ ◉ Goals ] | [ DYNAMIC CONTENT ]
                         |             |             |----------------------------------
                         |             |             | [ 🗓️ Month ]
                         |             |             | [ 📖 Subj ]
                         |             |             | [ (Cards, Charts, Forms, Lists) ]
                         |             |             | [ ◆ Skill ]
                         |             |             | [ ⚠️ Report ]
========================================================================================
                                DATA & RENDER PIPELINE                                  
========================================================================================
[ [ ] localStorage ] <=======> [ store{} State Management ] -------> [ render() Engine ]

---

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- That's it. Seriously. 🎉

### Installation

**Option 1 — Direct Download**
```bash
# Clone the repository
git clone https://github.com/devesh-tiw/StudyTracker.git

# Navigate to the project
cd studycore

# Open in your browser
open index.html
# or simply double-click the index.html file