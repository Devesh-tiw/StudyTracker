<div align="center">

<img src="https://raw.githubusercontent.com/Devesh-tiw/StudyTracker/main/S1.png" alt="StudyCore banner" width="100%" />

# ⬡ StudyCore

### A single-file, fully offline study dashboard for engineering students

*Plan your day, set weekly goals, map out the month, track subjects and skills, bookmark learning videos, and watch your progress add up — all client-side, no sign-up, no server.*

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)](https://www.chartjs.org/)

**[🚀 Live Demo](https://studydeveshtrack.netlify.app/)** · **[🐛 Report a Bug](https://github.com/Devesh-tiw/StudyTracker/issues)** · **[💡 Request a Feature](https://github.com/Devesh-tiw/StudyTracker/issues)**

</div>

---

## 📋 Table of Contents

- [About](#-about)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Project Structure](#-project-structure)
- [How Your Data Is Stored](#-how-your-data-is-stored)
- [Customizing the Theme](#-customizing-the-theme)
- [Browser Support](#-browser-support)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 About

**StudyCore** is a self-contained academic dashboard built as a single HTML file — no framework, no bundler, no backend. Open it in a browser and you get a complete study-management app: daily task planning, weekly goal tracking, a month-view planner, a subject library, a bookmarkable video-learning list, a skills/hobbies tracker, and a reports view that turns everything into charts.

Everything runs in the browser and saves to `localStorage`, so your data never leaves your device and the app works fully offline once loaded.

| Problem | StudyCore's answer |
|---|---|
| 🔴 Study plans scattered across notebooks, apps, and sticky notes | ✅ One dashboard for tasks, goals, the month, subjects, skills, and videos |
| 🔴 No real visibility into how you're actually studying | ✅ Streaks, achievements, and Chart.js visualizations of your activity |
| 🔴 Tools that need an account, a subscription, or an internet connection | ✅ Zero sign-up, zero cost, works fully offline |
| 🔴 Heavy tools with a learning curve | ✅ Open `index.html` and start typing |
| 🔴 "Where is my data actually stored?" | ✅ Nowhere but your own browser's `localStorage` |

---

## ✨ Features

### 🏠 Home / Dashboard
- Personal greeting with an editable name and a rotating motivational quote
- Live stat cards: today's tasks, completed count, active weekly goals, subject count
- 🔥 **Day streak** counter, calculated from consecutive days with at least one completed task
- 🏆 **Achievements** that unlock automatically — first completed task, 10/50 tasks done, 3- and 7-day streaks, 3 subjects added, a finished weekly goal, 5 bookmarked videos, 5 skills logged
- Weekly progress bar chart (tasks created vs. completed, last 7 days) and a subject-distribution doughnut chart
- Quick-add box for dropping a task in without leaving the dashboard

### ✅ Today's Focus (Day Tasks)
- Create tasks with title, subject, priority, date, and notes
- Three priority levels — 🔴 High, 🟡 Medium, 🟢 Low — with a priority-distribution doughnut chart
- Filter tasks by any date, toggle done/undone with one click, and track completion with a live progress bar

### 🎯 Weekly Goals
- Set custom targets (e.g. *"Complete 10 DSA problems"*) with `+1` / `-1` progress controls
- Weekly calendar strip showing tasks per day
- Horizontal bar chart comparing target vs. actual progress per goal, color-coded per goal

### 📅 Month Planner
- Click-to-plan interactive calendar with Previous/Next month navigation
- Tag plans as Study, Exam, Assignment, Lab, Project, or Revision
- Color-coded dots mark days with plans or tasks, plus a chronological plan list and a monthly task-distribution chart

### 📚 My Subjects
- Add subjects with name, code, and a custom color
- Per-subject completion percentage and progress bar
- Subjects you add here automatically populate every task/goal dropdown in the app

### 📺 Video Library
- Bookmark YouTube videos or playlists as a personal learning queue
- Track each as Not Started, In Progress, or Completed, with live stat cards and one-click filtering

### ⚡ Skills & Hobbies
- Log skills, hobbies, tools, languages, or favorite subjects with a custom icon
- Four mastery levels (Beginner → Intermediate → Advanced → Expert) shown as progress bars
- Radar chart of your overall skill spread once you've added 3+ skills

### 📊 My Progress (Reports)
- Four tabs: **Overview**, **By Subject**, **Daily Trend**, **Priority Analysis**
- Overview: total tasks, completion rate, and day streak at a glance
- Per-subject mini-charts, a 14-day activity trend, and a priority-level completion breakdown

### 🛡️ Data & Privacy
- Auto-saves to `localStorage` on every change — nothing is ever sent to a server
- "Reset All Data" with a confirmation prompt before it wipes anything
- Fully usable offline once the page has loaded once

---

## 🛠 Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Single-file structure and layout |
| **CSS3** | Custom properties (theming), Grid, Flexbox, animations |
| **Vanilla JavaScript** | All app logic, state management, and DOM rendering — no framework |
| **[Chart.js 4.4.1](https://www.chartjs.org/)** (via CDN) | Bar, line, doughnut, and radar charts |
| **Google Fonts** | Fraunces (headings), Plus Jakarta Sans (body), Space Mono (data/numbers) |
| **`localStorage` Web API** | 100% client-side data persistence |

There is no build step, no `package.json`, and no server — `index.html` is the entire application.

---

## 🚀 Getting Started

### Prerequisites
Just a modern browser (Chrome, Firefox, Edge, or Safari). That's it.

### Run it locally

```bash
# Clone the repository
git clone https://github.com/Devesh-tiw/StudyTracker.git

# Move into the project folder
cd StudyTracker

# Open the app — double-click index.html, or:
open index.html        # macOS
start index.html        # Windows
xdg-open index.html     # Linux
```

There's nothing to install and nothing to build — `index.html` loads Chart.js and Google Fonts from a CDN and runs entirely in your browser.

### Or just use the hosted version
No cloning needed — the app is live at **[studydeveshtrack.netlify.app](https://studydeveshtrack.netlify.app/)**. Your data still stays local to whichever browser you use it in.

---

## 📁 Project Structure

```
StudyTracker/
├── index.html   # The entire app — markup, CSS, and JS in one file
├── image.html   # SVG source for the banner graphic above
├── S1.png       # Rendered banner (used in this README)
└── README.md
```

---

## 💾 How Your Data Is Stored

StudyCore keeps a single JSON object in `localStorage` under the key `studycore_home_data`, shaped roughly like this:

```js
{
  userName: 'Student',
  tasks: [],          // day tasks
  weekGoals: [],       // weekly goals + progress
  monthPlans: {},      // calendar-keyed month planner entries
  subjects: [],        // subject list with colors/codes
  skills: [],          // skills & hobbies
  youtubeVideos: [],   // Video Library bookmarks
}
```

It's written back to `localStorage` on every change, so a refresh (or coming back tomorrow) picks up right where you left off — in that same browser, on that same device. Because nothing is synced anywhere, clearing your browser's site data or switching devices/browsers will start you with a clean slate.

---

## 🎨 Customizing the Theme

All colors live as CSS custom properties at the top of `index.html`:

```css
:root {
  --bg: #0f0a1e;
  --accent: #ffd93d;
  --accent2: #ff6b9d;
  --accent3: #6bcf7f;
  --accent4: #ffa552;
  --text: #f5f0ff;
  /* ...and more */
}
```

Swap these values to re-theme the whole app without touching any component markup.

---

## 🌐 Browser Support

Any evergreen browser with `localStorage` and modern CSS (Grid/Flexbox) support — current Chrome, Firefox, Edge, and Safari all work well.

---

## 🗺 Roadmap

A few directions this project could grow in — not yet built, just ideas:

- [ ] Export / import your data as JSON (for backup or moving between devices)
- [ ] Light theme toggle
- [ ] Installable PWA support for true offline app-like use
- [ ] Optional cloud sync for multi-device use

---

## 🤝 Contributing

This started as a personal tool, but issues and pull requests are welcome — bug reports, feature ideas, or UI polish all help. Open an [issue](https://github.com/Devesh-tiw/StudyTracker/issues) to start a conversation before a larger PR.

---

## 📄 License

No `LICENSE` file is included in this repository yet. Until one is added, please check with the repo owner before reusing or redistributing the code.

---

<div align="center">

Built by **[Devesh Tiwari](https://github.com/Devesh-tiw)**

</div>