# JSErrorFlow: Real-Time DOM Visualizer for JavaScript Debugging


[![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/ci.yml?style=flat-square&logo=githubactions)](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension?style=flat-square&logo=codecov)](https://codecov.io/gh/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension)
[![JavaScript](https://img.shields.io/badge/language-javascript-brightgreen?style=flat-square&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![TypeScript](https://img.shields.io/badge/language-typescript-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/framework-vite-purple?style=flat-square&logo=vite)](https://vitejs.dev/)
[![WXT](https://img.shields.io/badge/framework-wxt-orange?style=flat-square&logo=wxt)](https://wxt.dev/)
[![License](https://img.shields.io/github/license/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension?style=flat-square)](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension?style=flat-square&logo=github)](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension)

**JSErrorFlow** is a cutting-edge browser extension that visually highlights JavaScript errors directly on DOM elements in real-time. This developer tool streamlines frontend debugging, boosts productivity, and provides immediate, intuitive visual feedback to accelerate development cycles. Pinpoint and fix errors faster.

## 🚀 Features

*   **Real-Time Error Highlighting:** Errors are visualized directly on the affected DOM elements as they occur.
*   **Intuitive Visual Feedback:** Understand error context at a glance without deep console diving.
*   **Cross-Browser Compatibility:** Designed for Chrome and Firefox.
*   **Developer Productivity Boost:** Accelerate debugging and development cycles significantly.

---

## 🏛️ Architecture

mermaid
graph TD
    A[Browser Environment] --> B{JSErrorFlow Extension}
    B --> C[Content Script: DOM Monitoring & Error Detection]
    C --> D[Content Script: Error Visualization Logic]
    D --> E[Content Script: Direct DOM Manipulation]
    B --> F[Background Script: Event Handling & Messaging]
    F <--> G[Browser APIs]
    B --> H[Popup/Devtools Panel (Optional): Configuration & Summaries]
    H <--> G


## 📄 Table of Contents

*   [🚀 Features](#-features)
*   [🏛️ Architecture](#️-architecture)
*   [📄 Table of Contents](#-table-of-contents)
*   [🤖 AI Agent Directives](#-ai-agent-directives)
*   [🔧 Development Setup](#-development-setup)
*   [📦 Build & Development Scripts](#-build--development-scripts)
*   [🛡️ Principles](#️-principles)
*   [📜 License](#license)
*   [⭐ Support](#⭐-support)

---

## 🤖 AI Agent Directives

<details>
<summary><code>Expand for Agent Directives</code></summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**. This repository, `JSErrorFlow-Real-Time-Visualizer-Browser-Extension`, is a browser extension project.

*   **PRIMARY SCENARIO A: WEB / APP / EXTENSION (TypeScript/JavaScript)**
    *   **Stack:** This project leverages **TypeScript 6.x** and **JavaScript**. Key tools include **Vite 7 (Rolldown)** for fast builds, **WXT (Web Extension Tooling)** for streamlined extension development, and **Biome** for lightning-fast linting and formatting.
    *   **Architecture:** Employs a **Modular Architecture** suitable for browser extensions, with clear separation between content scripts, background scripts, and potential UI panels (like popups or devtools). Adheres to **Feature-Sliced Design (FSD)** principles where applicable for maintainable code organization.
    *   **Linting & Formatting:** **Biome** is mandated for code quality and consistency across the project. Its speed ensures minimal disruption to development velocity.
    *   **Testing:** **Vitest** is the standard for unit and component testing, integrated seamlessly with Vite. **Playwright** is mandated for end-to-end (E2E) testing to simulate real user interactions across different browser environments.
    *   **Styling:** **Tailwind CSS v4** is the preferred utility-first CSS framework for rapid UI development.

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Rust/Go) - *Not applicable.***
*   **TERTIARY SCENARIO C: DATA / AI / SCRIPTS (Python) - *Not applicable.***

---

## 4. OPERATIONAL PROTOCOLS
*   **CODE QUALITY & VERIFICATION:**
    *   **Strict Linting:** All code must pass Biome checks without errors or warnings.
    *   **Testing Coverage:** Maintain a minimum of **85% code coverage** via Vitest.
    *   **E2E Validation:** All critical user flows must pass Playwright E2E tests.
    *   **Type Safety:** **MANDATORY** TypeScript strict mode (`"strict": true`). Utilize `any` sparingly and only when absolutely necessary and justified.
    *   **Immutable State:** Prefer immutable data structures and state management patterns.
*   **DEVELOPMENT VELOCITY:**
    *   **Fast Feedback Loops:** Leverage Vite's HMR (Hot Module Replacement) for instantaneous UI updates.
    *   **Automated CI/CD:** Robust GitHub Actions workflows must execute on every push and pull request.
    *   **Dependency Management:** Utilize `npm` or `yarn` (with lockfiles) for predictable and reproducible builds.
*   **SECURITY:**
    *   **Dependency Auditing:** Regularly run `npm audit` or equivalent to identify and mitigate vulnerabilities.
    *   **Least Privilege:** Background and content scripts should only request the minimum necessary permissions.
    *   **Sanitization:** Implement robust input sanitization, especially for messages passed between scripts and from external sources.
    *   **Secrets Management:** **NEVER** hardcode secrets. Utilize environment variables or secure storage mechanisms provided by the browser extension framework.
*   **ARCHITECTURE & DESIGN:**
    *   **SOLID Principles:** Adhere to SOLID principles in all code design.
    *   **DRY (Don't Repeat Yourself):** Avoid code duplication.
    *   **YAGNI (You Ain't Gonna Need It):** Implement only what is currently required.
*   **COMMUNICATION:**
    *   **Clear Commit Messages:** Follow Conventional Commits standard (`feat:`, `fix:`, `chore:`, etc.).
    *   **Meaningful PR Descriptions:** Detail changes, rationale, and testing performed.

---

## 5. STANDARD 11 MANDATE
All repositories **MUST** adhere to the following professional standards:
1.  **README.md:** Comprehensive project overview, setup, and usage.
2.  **PROPOSED_README.md:** Draft for review based on AGENTS.md.
3.  **badges.yml:** Configuration for dynamic badges.
4.  **LICENSE:** Specify the license (CC BY-NC 4.0).
5.  **.gitignore:** Standard ignore file for the tech stack.
6.  **.github/workflows/ci.yml:** CI/CD pipeline configuration.
7.  **.github/CONTRIBUTING.md:** Guidelines for contributors.
8.  **.github/ISSUE_TEMPLATE/*:** Issue templates for bug reports, features, etc.
9.  **.github/PULL_REQUEST_TEMPLATE.md:** PR template.
10. **.github/SECURITY.md:** Security policy and reporting.
11. **AGENTS.md:** This document, detailing the AI Agent's directives.

---

## 6. PRODUCTIVITY ENHANCEMENTS
*   **Live Reloading:** Vite's HMR ensures instant feedback.
*   **Automated Testing:** Vitest and Playwright catch regressions early.
*   **Linters & Formatters:** Biome enforces consistent code style.

</details>

---

## 🔧 Development Setup

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension.git
    cd JSErrorFlow-Real-Time-Visualizer-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    npm install
    # or
    yarn install
    

3.  **Run in Development Mode:**
    This command starts the Vite development server and builds the extension in watch mode. You can then load the extension in your browser (e.g., Chrome, Firefox) from the `dist` folder.
    bash
    npm run dev
    # or
    yarn dev
    

4.  **Run Linters & Formatters:**
    Ensure your code adheres to the project's coding standards.
    bash
    npm run lint
    # or
    yarn lint
    

5.  **Run Tests:**
    Execute unit and E2E tests.
    bash
    npm test
    # or
    yarn test
    

---

## 📦 Build & Development Scripts

| Script      | Description                                           |
| :---------- | :---------------------------------------------------- |
| `dev`       | Start development server with hot module replacement. |
| `build`     | Build the extension for production.                   |
| `preview`   | Locally preview production build.                     |
| `lint`      | Run Biome linter and formatter.                       |
| `test`      | Run Vitest unit tests.                                |
| `test:e2e`  | Run Playwright end-to-end tests.                      |
| `coverage`  | Generate code coverage report.

---

## 🛡️ Principles

This project is built upon the following core software engineering principles:

*   **SOLID:** Designing for maintainability and extensibility.
*   **DRY (Don't Repeat Yourself):** Avoiding redundant code.
*   **YAGNI (You Ain't Gonna Need It):** Focusing on current requirements.
*   **KISS (Keep It Simple, Stupid):** Favoring straightforward solutions.

---

## 📜 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the [LICENSE](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/blob/main/LICENSE) file for more details.

---

## ⭐ Support

If you find this project valuable, please consider starring the repository on GitHub! Your support fuels future development.

[<img src="https://img.shields.io/github/stars/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension?color=blue&label=Star%20on%20GitHub&logo=github" alt="Star on GitHub" />](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/stargazers)
