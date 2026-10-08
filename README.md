# Girish Balaso Lade — Systems Engineer & Founder Portfolio

A high-performance, single-file responsive portfolio website for **Girish Balaso Lade** (Systems Engineer & Founder of **LadeStack**). 

Engineered strictly according to the **Zapier Design System** specification, this website blends a warm-cream canvas (`#fffefb`), deep coffee-ink typography (`#201515`), and a single saturated Zapier orange (`#ff4f00`) conversion CTA with a universal 12px border radius.

---

## 📑 Table of Contents

- [Overview](#overview)
- [Design System & Tokens](#design-system--tokens)
- [Key Features](#key-features)
- [Sections Breakdown](#sections-breakdown)
- [Architecture & Tech Stack](#architecture--tech-stack)
- [Getting Started](#getting-started)
- [Deployment](#deployment)
- [Customization Guide](#customization-guide)
- [License & Attribution](#license--attribution)

---

## 🌟 Overview

This portfolio showcases Girish Lade's profile, engineering trajectory, venture ecosystem, projects, and verifiable open-source metrics. Built as a **zero-build, standalone single-file web application** (`index.html`), it requires no bundlers, compilation steps, or complex tooling.

### Highlights
- **Single-File Architecture**: All HTML structure, Tailwind CSS configuration, custom CSS scrollbars, and vanilla JavaScript logic live inside `index.html`.
- **Zapier Design Language**: Faithfully reproduces Zapier’s warm editorial aesthetic, balanced between developer precision and executive maturity.
- **Fully Responsive**: Mobile-first architecture with dedicated drawer navigation, touch-friendly heatmaps, and adaptive grids for tablet and desktop viewports.
- **Dynamic Interactions**: Features an algorithmic 52-week contribution matrix generator, clipboard copying with toast alerts, and smooth navigation.

---

## 🎨 Design System & Tokens

The interface implements the full Zapier marketing design token specification:

### 1. Color Palette

| Token | Hex Code | Purpose |
|---|---|---|
| `primary` | `#ff4f00` | Saturated Zapier Orange CTA & active accents |
| `primary-hover` | `#e54600` | Hover state for primary interactive elements |
| `canvas` | `#fffefb` | Warm cream page background (never cold pure white) |
| `canvas-soft` | `#f8f4f0` | Inset cream surface for cards, timeline & metadata |
| `ink` | `#201515` | Deep coffee heading & primary text (never pure black) |
| `ink-soft` | `#2f2a26` | Near-black secondary headings with brown warmth |
| `ink-mid` | `#36342e` | Mid-emphasis text |
| `body` | `#605d52` | Default body copy |
| `body-mid` | `#939084` | Captions, dates & secondary metadata |
| `mute` | `#c5c0b1` | Fine print, low-emphasis captions & zero-commit heatmap cells |

### 2. Typography

- **Display & Headings**: Inter (weight 500/600/700) rendered in sentence-case (never all-caps for display).
- **Eyebrows**: Degular-style uppercase labels with positive letter-spacing (`tracking-[1px]`).
- **Code & Metadata**: `JetBrains Mono` for badges, tags, metrics, and terminal elements.

### 3. Geometry & Elevation

- **Universal Radius (`rounded-[12px]`)**: Cards, inputs, and buttons uniformly share a 12px radius — positioned deliberately between rounded pills and sharp technical boxes.
- **Hairline Chrome**: 1px subtle borders (`border-ink/10` to `border-ink/15`) and surface contrast provide depth without heavy artificial drop shadows.
- **Polarity-Flipped Dark Footer**: High-contrast footer styled in dark coffee ink (`#201515`) with warm off-white text.

---

## ⚡ Key Features

- **Responsive Mobile Navigation**:
  - Hamburger toggle with animated icon switching (`fa-bars` $\leftrightarrow$ `fa-xmark`).
  - Auto-collapsing drawer on menu link click.
  - Floating back-to-top button that reveals automatically on downward scroll.

- **Interactive Copy-to-Clipboard**:
  - Instant one-click email copying (`girishlade111@gmail.com`).
  - Animated floating toast notification with timeout dismissal.

- **Dynamic 52-Week Contribution Heatmap**:
  - Algorithmic generative grid calculating 364 days of simulated commit activity.
  - Uses Zapier orange scale intensities (`bg-mute/40` $\rightarrow$ `bg-primary`).
  - Mobile horizontal scroll container with intuitive swipe guidance.

- **Verified Profile Credentials**:
  - Displays GitHub achievements (Pull Shark, Quickdraw, Arctic Code Vault, Starstruck).
  - Production-validated language breakdown bar with exact distribution percentages.

---

## 🧭 Sections Breakdown

1. **Header & Navigation**: Fixed brand identity, desktop anchor links, quick GitHub follow button, primary contact CTA, and mobile drawer.
2. **Hero Section**: Profile avatar, age identifier (20 y/o), role tag, core bio, status badge, location marker, and quick tech chips.
3. **Core Beliefs & Philosophy**: Quotation and manifesto card highlighting system resilience, engineering velocity, and high leverage.
4. **The Trajectory**: Vertical milestone timeline tracing computer science foundations, full-stack development, distributed systems, and founding LadeStack.
5. **LadeStack Ecosystem**: 6-card venture grid displaying:
   - *LadeStack Core* (Backend Agent Engine & Gateway)
   - *LadeFlow* (Visual Pipeline & Automation Tool)
   - *MicroLog* (Zero-Allocation Telemetry Library)
   - *CloudNest* (Distributed Object Storage Engine)
   - *SystemDesignNotes* (Architecture Blueprints & Diagrams)
   - *CodeVault* (Algorithms & Design Patterns Repository)
6. **Featured Projects**: Deep-dive codebases with star counts, stack tags, repository links, and architecture spec buttons.
7. **Tech Stack**: Three organized capability buckets (Languages, Backend & Systems, Frontend & Tooling).
8. **Currently Grinding**: In-progress research areas (Raft/Paxos consensus, Kafka internals, Linux epoll concurrency, multi-region scaling).
9. **Verifiable GitHub Activity**: Aggregated lifetime statistics (16,000+ lines, 35+ repos, 157+ commits, 42-day streak), 52-week heatmap, and language distribution.
10. **Connect Card**: Direct connection channels (GitHub, LinkedIn, X/Twitter, direct email) and remote role availability indicator.
11. **Footer**: Polarity-flipped dark coffee bar with copyright, status, and navigation anchors.

---

## 🛠️ Architecture & Tech Stack

The project requires **no build step** and loads dependencies via secure CDNs:

- **Tailwind CSS v3 (JIT CDN)**: Configured in-head with custom Zapier color palettes and radius tokens.
- **Font Awesome 6.5.1**: Scalable icon set for technical brands and action buttons.
- **Google Fonts**:
  - `Inter`: Weights 400, 500, 600, 700
  - `JetBrains Mono`: Weights 400, 500, 600
- **Vanilla JavaScript (ES6+)**:
  - Clipboard API fallback
  - Dynamic contribution grid computation
  - Scroll listener with debounce for the floating back-to-top button
  - Mobile navigation drawer toggle

---

## 🚀 Getting Started

### Prerequisites

All you need is a modern web browser (Google Chrome, Firefox, Safari, Microsoft Edge, Brave).

### Local Execution

1. Clone or download the repository:
   ```bash
   git clone https://github.com/girishlade111/portfolio.git
   cd portfolio
   ```

2. Open `index.html` directly:
   - Double-click `index.html` in your file explorer, OR
   - Run a local static file server using Python:
     ```bash
     # Python 3.x
     python -m http.server 8000
     ```
   - Open your browser at `http://localhost:8000`.

---

## 🌐 Deployment

Because the website consists of a single static `index.html` file, it can be deployed for free in seconds:

### Option 1: GitHub Pages
1. Push `index.html` to the root of your GitHub repository.
2. Go to **Settings** $\rightarrow$ **Pages**.
3. Under **Build and deployment**, select **Source: Deploy from a branch**.
4. Choose branch `main` and folder `/ (root)`, then click **Save**.
5. Your portfolio will be live at `https://<your-username>.github.io/<repo-name>/`.

### Option 2: Vercel / Netlify
- Drag and drop the folder containing `index.html` directly onto the [Vercel](https://vercel.com) or [Netlify](https://netlify.com) dashboard for zero-configuration instantaneous deployment.

---

## ✏️ Customization Guide

To modify this portfolio for your own profile or update Girish's projects:

### 1. Update Personal Information
Open `index.html` and search for the following entries:
- **Name & Title**: Update `Girish Balaso Lade` and `Systems Engineer & Founder @ LadeStack`.
- **Avatar Image**: Replace `https://avatars.githubusercontent.com/u/108502392?v=4` with your preferred image URL.
- **Social Handles**: Search for `girishlade111` or `girishlade` and swap with your profile usernames.

### 2. Update Email & Contact Action
In `index.html`, locate the `copyEmailToClipboard()` function:
```javascript
function copyEmailToClipboard() {
    const email = "your-email@example.com"; // <-- Update email address here
    // ...
}
```

### 3. Add or Modify Ecosystem Products
In the `#ecosystem` section, duplicate or edit any of the 6 card containers inside the `grid-cols-1 md:grid-cols-2 lg:grid-cols-3` layout.

---

## 📄 License & Attribution

Designed and engineered for **Girish Balaso Lade**.  
Aesthetic style inspired by the Zapier Brand & Marketing Design System.

Licensed under the [MIT License](https://opensource.org/licenses/MIT). You are free to fork, adapt, and use this template for personal portfolios.
