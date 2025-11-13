# IA382 — AI-Enhanced Practical Tutorials (Docker & Kubernetes) 🚀

[![Live Demo](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen)](https://fernando-sant.github.io/ia382-containers-196990/)
[![Made with ❤️ + 🤖](https://img.shields.io/badge/made%20with-%E2%9D%A4%EF%B8%8F%20%2B%20%F0%9F%A4%96-blueviolet)](#)
[![Static Site](https://img.shields.io/badge/site-static-orange)](#)
[![License](https://img.shields.io/badge/license-GPL--3.0-blue)](https://www.gnu.org/licenses/gpl-3.0.en.html)

**👉 Live site:**  
**https://fernando-sant.github.io/ia382-containers-196990/**

> A collection of practical, interactive tutorials for the **IA382** course at FEEC/UNICAMP, focusing on Docker, Docker Compose, and Kubernetes — designed with AI assistance to deliver a consistent, modern, and accessible UX.

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [✨ Features](#-features)
- [📚 Modules](#-modules)
- [📦 Activity Files](#-activity-files)
- [🧭 How to Use](#-how-to-use)
- [🤖 The Role of AI](#-the-role-of-ai)
- [🛠️ Stack & Structure](#️-stack--structure)
- [🧪 Tips & Troubleshooting](#-tips--troubleshooting)
- [🙌 Credits](#-credits)

---

## 🧠 About the Project

This static website was created by **Fernando Santiago (196990)** using **AI-assisted development techniques** for the 2S/2025 IA382 Course.  
The goal: transform raw, unstyled HTML tutorials into a **cohesive, interactive learning platform** with light/dark mode, automatic TOC, copy buttons on code snippets, and subtle animations.

---

## ✨ Features

- 🎨 **Consistent, professional design** across all modules.  
- 🌓 **Persistent Light/Dark Theme Switcher** (remembers user choice).  
- 🧭 **Dynamic TOC (scroll-spy):**
  - Auto-generates from `h2`/`h3` headings.  
  - Highlights the active section while scrolling.  
  - Smooth scroll to view and visual hierarchy.  
- 📋 **Code Blocks with “Copy” Button** and visual confirmation.  
- 📱 **Fully Responsive Design** for mobile, tablet, and desktop.  
- ♿ **Enhanced Accessibility** (keyboard focus, semantic headings, color contrast).  
- 🔗 **Next/Previous Navigation** between modules.  
- 🧩 **Reusable structure** ready for new tutorial pages.

---

## 📚 Modules

Each page follows the same visual and pedagogical structure:

- 🏠 **[Index](index.html)** — main landing page.  
- 🛠️ **[Installing Docker](ia382_install_docker.html)** — step-by-step installation guide (Windows, macOS, Ubuntu).  
- ▶️ **[Running Containers](ia382_running_containers.html)** — basics of `docker run`, process management, and networking.  
- 🐾 **[Compose & Kubernetes: Pet Store](ia382_compose_petstore.html)** — introduction to Docker Compose and Kubernetes concepts.  
- 🍽️ **[Lab: TripMeal](ia382_tripmeal.html)** — final hands-on lab integrating Compose and Kubernetes.  

> Every page includes a sidebar TOC, dark/light mode, and pagination controls.

---

## 📦 Activity Files

Tutorials include downloadable `.zip` archives used in exercises, located in the `activities_files/` folder:

- `activities_files/pet-store.zip`  
- `activities_files/tripmeal.zip`  
- `activities_files/word-frequency.zip`

> Links inside tutorials point directly to these files.

---

## 💻 How to Use

No backend server required — it’s a fully static website.

```bash
# 1) Clone the repository
git clone https://github.com/fernando-sant/ia382-containers-196990.git
cd ia382-containers-196990

# 2) (Optional) Serve locally for better relative path handling
python -m http.server 8080
# Open: http://localhost:8080
```

Alternatively, simply open `index.html` in your browser.

---

## 🤖 The Role of AI

This project also served as an experiment in **human–AI collaboration**.

- **Scaffolding & Refactor:** AI generated the base CSS/JS and applied consistent styling across multiple pages.  
- **Microinteractions & Accessibility:** Implemented scroll spy, copy buttons, and improved focus visibility.  
- **Batch Refactoring:** Automated repetitive transformations (“Do the same for this HTML”) across the tutorial set.  
- **Contextual Generation:** AI inferred new page structures (e.g., homepage) using context from existing ones.  
- **Pair Debugging:** Example prompt → “The TOC is too tall.” → AI fix → `max-height` and `overflow-y` adjustments.

**Outcome:** huge productivity boost — what would take days was achieved in one session.  
The AI’s greatest value wasn’t *creating* from scratch, but *transforming and modernizing* content efficiently.

---

## 🛠️ Stack & Structure

**Stack:** Pure HTML + CSS + vanilla JS.  
**Key idea:** every HTML file includes a unified `<style>` and `<script>` section (theme switcher, TOC, copy buttons).

**Structure:**

```
ia382-containers-196990/
├─ index.html
├─ ia382_install_docker.html
├─ ia382_running_containers.html
├─ ia382_compose_petstore.html
├─ ia382_tripmeal.html
└─ activities_files/
   ├─ pet-store.zip
   ├─ tripmeal.zip
   └─ word-frequency.zip
```

To **add new modules**, duplicate an existing page and replace only the `<main>` content.

---

## 🧪 Tips & Troubleshooting

- **TOC too tall?** Already handled with `max-height` and `overflow-y: auto`.  
- **Theme not persisting?** Check browser’s `localStorage`.  
- **Broken links?** Ensure filenames and `.zip` paths match.  
- **Serving via HTTP:** Some APIs (e.g., clipboard) may require running via a local server.  

---

## 🙌 Credits

- Educational content adapted and expanded for **IA382 / FEEC–UNICAMP**.
- Inspired by the third seminar (2S/2025) **Performance Analysis of Lightweight Container Orchestration Platforms for Edge-Based IoT Applications**  
- Base material adapted from **G. Schenker, “Learn Docker — Fundamentals of Docker 19.x” (2020)**, chapters 14 & 20.  
- Modern front-end and UX refined using **AI tools**.  

---

> 💡 *This repository demonstrates how AI can assist not just in code generation, but in creating cohesive, elegant, and maintainable educational tools.*

## 🧾 License

This project is licensed under the **GNU General Public License v3.0 (GPL-3.0)** —  
you are free to use, modify, and distribute it under the same terms.  

📄 Read the full license text here:  
https://www.gnu.org/licenses/gpl-3.0.en.html
