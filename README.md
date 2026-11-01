# MindLoop — Clinical Mental Health Monitoring Platform

Understand the patient beyond the appointment.

MindLoop connects patient daily experiences, passive wearable biometrics, and AI-assisted observations to bridge the 30-day consultation gap for psychiatrists.

---

## Quick Start (Local Setup)

### 1. Prerequisites
- **Node.js** (v18.0.0 or higher recommended, e.g., Node 20 LTS)
- **npm** (comes with Node.js) or **yarn** / **pnpm** / **bun**

### 2. Extract and Enter Directory
Extract the downloaded ZIP file, open your terminal (Command Prompt, PowerShell, or macOS Terminal), and navigate into the folder:
```bash
cd mindloop
```

### 3. Install Dependencies
```bash
npm install
```
*(If your local npm version throws peer dependency warnings, use `npm install --legacy-peer-deps`)*

### 4. Run Development Server
```bash
npm run dev
```

Your app will be running locally at:
👉 **`http://localhost:3000`** (or the port shown in your terminal).

---

## Available Commands

- `npm run dev`: Starts the Vite development server with hot reload.
- `npm run build`: Builds production-ready static assets in the `dist/` directory.
- `npm run preview`: Previews the built production app locally.
- `npm run lint`: Runs TypeScript validation checks (`tsc --noEmit`).

---

## Dual Portal Architecture

- **Psychiatrist Clinical Portal (`/doctor`)**:
  - Cohort triage status (Routine, Review Recommended, Prompt Review)
  - 30-day longitudinal multivariate SVG charts (Mood vs Stress, Sleep vs Activity)
  - Interactive click-to-date raw evidence drilldown
  - 5-part AI observations citing supporting dates
  - Action logger & alert acknowledgement
- **Patient Wellness Portal (`/patient`)**:
  - Standardized evening clinical assessment
  - Conversational journal with transparent structured entity review
  - Continuous biometric hardware sync (Titanium smartwatch telemetry)
  - Care team connection and 988 emergency escalation directives
- **Judge Demonstration Track**:
  - Interactive 10-step presenter toolbar anchored at the bottom for seamless hackathon presentations.
