# 🌍 Explore World Travels — Static Team Website


A premium, highly responsive static travel portal constructed collaboratively as part of our **Week 3 Git Flow Assignment**. The project implements isolated feature branch development, pull request code reviews, and centralized version integration.

🌐 **Live Production Link:** (https://arunabhilashm.github.io/collaborative-static-website/)

---

## 📋 Project Architecture & File Structure

The workspace consists of a clean semantic asset tree sharing a single, deeply isolated master stylesheet:

```text
week3-git-flow/
├── index.html                # Travel Homepage & Popular Destinations
├── about.html                # Core Mission, Values & Destination Grid
├── contact.html              # Corporate Headquarters Contact Panel
└── styles.css                # Global Unified Master Stylesheet (CSS3)
```

---

## 🚀 DevOps Team Task Division

### 👤 MEMBER 1: Project Admin & Homepage Lead (Arun)
*   **Branch**: `homepage`
*   **Code Responsibility**: Modifies `index.html` [INDEX].
*   **DevOps Duty**: Created the central GitHub repository, invited all collaborators, configured the GitHub Pages hosting channel, and manages the final merge into `main`.

### 👤 MEMBER 2: UI Designer & CSS Architect (Preethi)
*   **Branch**: `global-styling`
*   **Code Responsibility**: Created the master `styles.css`.
*   **DevOps Duty**: Architected the core layout theme (premium colors, typography modules, floating glass card cards, and navbar aesthetics) to ensure global website cohesiveness.

### 👤 MEMBER 3: About Page Developer (Darun)
*   **Branch**: `about-page`
*   **Code Responsibility**: Created `about.html`.
*   **DevOps Duty**: Audited Member 1's initial Pull Requests and served as the project baseline for a successful "clean merge" pipeline execution into `develop`.

### 👤 MEMBER 4: Contact Page Developer & Conflict Fixer (Bharat)
*   **Branch**: `contactpage`
*   **Code Responsibility**: Created `contact.html`.
*   **DevOps Duty**: Intentionally edited lines inside the global CSS system simultaneously alongside other branches to trigger, track, fix, and demonstrate the assignment's mandatory merge conflict resolution workflow.

---

## 🛠️ Version Control Workflow (Git Flow)

This project strictly utilizes the **Git Flow** strategy to coordinate multi-user integrations seamlessly:

### 1. Repository Initializing
```bash
git clone https://github.com/ArunAbhilashM/collaborative-static-website.git
cd week3-git-flow
```

### 2. Feature Development Workflow Example
Each developer spun up a local branch to process changes safely without bleeding into operational production spaces:
```bash
git checkout -b global-styling
# UI Styling additions performed...
git add styles.css
git commit -m "style: finalize premium UI layouts and typography components"
git push origin global-styling
```

### 3. Merging & Integration
All features were integrated using GitHub Pull Requests directed solely to the **`develop`** base pipeline for code evaluation and review before deployment.

---

## 💥 Overcoming Engineering Challenges

*   **Roadblock: Unrelated History Rejections (`fatal: refusing to merge unrelated histories`)**
    *   *Cause*: Multi-member branches initialized their file workspaces separate from the repository's base core tracking stream.
    *   *Resolution*: Overrode Git security settings explicitly using the command pipeline loop flag:
        ```bash
        git pull origin feature/contact-page --allow-unrelated-histories
        ```
*   **Roadblock: CSS Grid Inheritance Collapses**
    *   *Cause*: Universal layout tags like `body > div` built for the About Page structural grids leaked onto the Contact layout, crushing the column elements vertically.
    *   *Resolution*: Implemented isolated component nesting selectors combined with explicit styling parameters to separate page styling rules completely.
*   **Roadblock: Typographical Text Line Breaks**
    *   *Cause*: Long string travel email parameters ran out of container boundaries, awkwardly dropping trailing single characters downward.
    *   *Resolution*: Bound content fields inside a strict wrapper layout with optimized padding scaling paired with:
        ```css
        word-break: break-word;
        overflow-wrap: break-word;
        ```

---
*Developed collaboratively by Arun, Preethi, Darun, and Bharat — 2026.*
