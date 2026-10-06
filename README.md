# Anshuman Gupta — Modern Recruiter-Focused Developer Portfolio

A modern, high-performance, dark-first developer portfolio engineered for **Anshuman Gupta** (B.Tech Computer Science Student at GLA University & Aspiring Software Development Engineer).

Built using **React + Vite + Tailwind CSS + Lucide Icons**.

---

## 🌟 Key Highlights & Design Decisions

- **Recruiter-First Layout**: Engineered to communicate *Who I am → What I build → Technologies → Accomplishments → Contact & Resume* in under 30 seconds.
- **Strictly Authentic**: Every metric, project, and certification is 100% sourced from Anshuman's latest resume and training credentials.
- **Deep Packet Inspection Blocker (Featured Project)**: Showcases C#, ASP.NET Core, WinDivert, and TLS SNI network packet filtering with an interactive pipeline visualization.
- **JanSeva Civic Portal (Featured Project)**: Highlights React.js, Tailwind CSS, and role-based dashboard architecture with live demo integration.
- **Centralized Data Layer**: All profile data, projects, skills, education, and achievements are organized in `src/data/portfolioData.js` for effortless one-file updates.
- **Responsive & Accessible**: Optimized for mobile phones, tablets, laptops, and ultra-wide screens with full `prefers-reduced-motion` compliance.

---

## 🛠️ Tech Stack

- **Framework**: React 18
- **Build Tool**: Vite 6 (Fast HMR & Optimized Bundles)
- **Styling**: Tailwind CSS (Custom Dark Slate/Cyan/Indigo Design System)
- **Icons**: Lucide React
- **Deployment**: Static SPA (Compatible with Netlify, Vercel, GitHub Pages, Render)

---

## 📁 Project Structure

```text
anshuman-portfolio/
├── public/
│   ├── favicon.svg                # Custom SVG brand favicon
│   ├── Anshuman-Gupta-Resume.pdf  # Authoritative Resume PDF
│   └── assets/                    # Project screenshots & profile images
│       ├── profile.jpg
│       ├── janseva.png
│       ├── weather.png
│       ├── qrcode.png
│       └── expense.png
├── src/
│   ├── main.jsx                   # React entry point
│   ├── App.jsx                    # Root app assembling all sections
│   ├── index.css                  # Design tokens, custom scrollbars, glowing borders
│   ├── data/
│   │   └── portfolioData.js       # ⚡ Central single source of truth for all content
│   └── components/
│       ├── Navbar.jsx             # Sticky navbar with active section scrollspy
│       ├── Hero.jsx               # Hero section with interactive terminal & CTAs
│       ├── StatsBanner.jsx        # Quick 30-second recruiter numbers
│       ├── About.jsx              # Bio narrative, philosophy & quick facts
│       ├── Skills.jsx             # Categorized skill badges with filter tabs
│       ├── Projects.jsx           # Flagship DPI Blocker & JanSeva showcase + utility grid
│       ├── Experience.jsx         # 6-Month DevsLane Full-Stack Training timeline
│       ├── Education.jsx          # GLA University & De Paul School history
│       ├── Achievements.jsx       # LeetCode 250+, SIH 2025, DevsLane & Java certifications
│       ├── CodingProfiles.jsx     # LeetCode and GitHub activity highlights
│       ├── ResumeSection.jsx      # Resume download and instant view CTA
│       ├── Contact.jsx            # Validated recruiter message form + direct email/phone copy
│       └── Footer.jsx             # Developer footer & back-to-top control
├── index.html
├── package.json
├── tailwind.config.js
└── vite.config.js
```

---

## 🚀 How to Run Locally

### 1. Prerequisites
- Node.js (v18.0.0 or later recommended)
- npm or yarn

### 2. Installation
Navigate into the project directory and install dependencies:
```bash
cd anshuman-portfolio
npm install
```

### 3. Start Development Server
```bash
npm run dev
```
Open your browser at `http://localhost:3000` (or the port specified in terminal).

---

## 📦 How to Build for Production

To create an optimized production build:
```bash
npm run build
```
The compiled static assets will be output to the `dist/` directory.

To test the production build locally:
```bash
npm run preview
```

---

## 🌐 Deployment Instructions

### Option 1: Deploy to Netlify (Recommended)
1. Push your repository to GitHub.
2. Log into [Netlify](https://app.netlify.com/).
3. Click **"Add new site"** → **"Import an existing project"** → Select your GitHub repository.
4. Set the build settings:
   - **Build Command**: `npm run build`
   - **Publish directory**: `dist`
5. Click **"Deploy site"**.

### Option 2: Deploy to Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in the project root and follow the quick interactive prompts.

### Option 3: Deploy to GitHub Pages
1. Install `gh-pages`: `npm install --save-dev gh-pages`
2. In `vite.config.js`, set `base: '/<repository-name>/'`.
3. Add deploy script in `package.json`: `"deploy": "gh-pages -d dist"`
4. Run `npm run build && npm run deploy`.

---

## ✏️ How to Easily Update Your Portfolio Later

All website content is intentionally isolated in **`src/data/portfolioData.js`**. You do **not** need to touch any UI components to update your information:

1. **Add a new Project**: Add a new object to the `projectsData` array in `src/data/portfolioData.js`.
2. **Add a new Skill**: Add a skill object to the relevant category in `skillsData`.
3. **Update LeetCode Count**: Update `stats` and `achievementsData` in `src/data/portfolioData.js`.
4. **Update Resume**: Replace `public/Anshuman-Gupta-Resume.pdf` with your new PDF file.
