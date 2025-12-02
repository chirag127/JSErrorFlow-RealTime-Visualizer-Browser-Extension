# JSErrorFlow-Real-Time-Visualizer-Browser-Extension

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/ci.yml?style=flat-square&logo=githubactions)](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/actions)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension?style=flat-square&logo=codecov)](https://codecov.io/gh/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension)
[![Tech Stack](https://img.shields.io/badge/built%20with-TypeScript%2C%20Vite%2C%20WXT-blue?style=flat-square&logo=typescript)](https://github.com/vitejs/vite) 
[![License](https://img.shields.io/github/license/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension?style=flat-square&logo=opensourceinitiative)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension?style=flat-square&logo=github)](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension)

**JSErrorFlow** is a cutting-edge browser extension that visually highlights JavaScript errors directly on DOM elements in real-time, transforming frontend debugging into an intuitive, immediate visual experience. This developer tool significantly streamlines debugging, boosts productivity, and accelerates development cycles by enabling developers to pinpoint and resolve errors faster than ever before.

## Table of Contents

*   [About the Project](#about-the-project)
*   [Key Features](#key-features)
*   [Architecture Overview](#architecture-overview)
*   [Getting Started](#getting-started)
*   [Development Workflow](#development-workflow)
*   [AI Agent Directives](#ai-agent-directives)
*   [Contributing](#contributing)
*   [License](#license)

## About the Project

In the fast-paced world of frontend development, quickly identifying and resolving JavaScript errors is paramount. JSErrorFlow provides an immediate, visual layer over your application's DOM, directly indicating where errors are occurring. Instead of sifting through console logs, developers can see errors manifested directly on the problematic elements, drastically reducing the time spent on debugging and increasing overall development velocity.

## Key Features

*   **Real-time DOM Error Highlighting:** Visual cues on elements that trigger JavaScript errors.
*   **Intuitive Debugging:** Immediate visual feedback eliminates guesswork.
*   **Cross-Browser Compatibility:** Supports Chrome and Firefox.
*   **Developer-Focused:** Designed to integrate seamlessly into existing development workflows.
*   **Performance Optimized:** Built with Vite for lightning-fast build times.

## Architecture Overview

mermaid
graph TD
    A[Browser Environment] --> B(WXT Framework)
    B --> C(Content Script)
    C --> D{DOM Monitoring & Error Interception}
    D --> E(Visual Overlay Injection)
    E --> F[User Interface]
    B --> G(Background Script)
    G --> H(API Communication - e.g., Error Reporting)
    F -.-> G


This extension adopts a modern architecture centered around the [WXT (WebExtension Tooling)](https://github.com/wxt-dev/wxt) framework, leveraging TypeScript for type safety and Vite for rapid development. The core logic is split between content scripts, which interact directly with the webpage's DOM, and background scripts, which manage extension-wide state and communication.

## Getting Started

### Prerequisites

*   Node.js 18+ 
*   npm or yarn

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension.git
    cd JSErrorFlow-Real-Time-Visualizer-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    npm install
    # or
    # yarn install
    

3.  **Run in Development Mode:**
    WXT provides commands to run the extension in development mode, allowing for hot module replacement.
    bash
    npm run dev
    # or
    # yarn dev
    

    Follow the instructions in your browser to load the unpacked development extension.

### Build for Production

To create a production-ready build for Chrome and Firefox:

bash
npm run build
# or
# yarn build


This will generate distributable packages in the `dist` directory.

## Development Workflow

*   **Core Technologies:** TypeScript, Vite, WXT, TailwindCSS (v4.0+).
*   **Linting & Formatting:** Biome for ultra-fast static analysis and code formatting.
*   **Testing:** Vitest for unit and integration tests, Playwright for end-to-end (E2E) testing.
*   **Architecture:** Feature-Sliced Design (FSD) principles for modularity and maintainability.

**Scripts:**

| Script        | Description                                     |
|---------------|-------------------------------------------------|
| `npm run dev` | Starts the development server with hot reloading. |
| `npm run build` | Builds the extension for production.            |
| `npm run lint`  | Runs Biome linter.                              |
| `npm run format`| Runs Biome formatter.                           |
| `npm run test`  | Runs Vitest unit and integration tests.         |
| `npm run test:e2e` | Runs Playwright E2E tests.                      |

**Principles:**

*   **SOLID:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
*   **DRY:** Don't Repeat Yourself.
*   **YAGNI:** You Ain't Gonna Need It.

## AI Agent Directives

<details>
<summary>Click to expand AI Agent Directives</summary>

## SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** Senior Principal Software Architect, Master Technical Copywriter with 40+ years of elite industry experience. Operating with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. Building for the 2026 standard.
**Output Standard:** EXECUTION-ONLY results. No plans; only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. Must **INFER** technical intent based on project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect project type (`package.json` for JS/TS) and apply **Apex Toolchain**.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript) - *This Repository Context***
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), WXT (WebExtension Tooling 1.x), TailwindCSS v4.0+.
    *   **State Management:** Signals (Standardized).
    *   **Linting & Formatting:** Biome v2.x (Ultra-fast static analysis).
    *   **Testing:** Vitest (Unit/Integration), Playwright (E2E).
    *   **Architecture:** Feature-Sliced Design (FSD).

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Rust/Go) - *Not applicable here.***

*   **TERTIARY SCENARIO C: DATA / SCRIPTS / AI (Python) - *Not applicable here.***

### 4. APEX NAMING CONVENTION (STAR VELOCITY ENGINE)
**Formula:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>`
**Format:** `Title-Case-With-Hyphens` (e.g., `JSErrorFlow-Real-Time-Visualizer-Browser-Extension`).

### 5. REPOSITORY INTEGRITY & PURPOSE PIVOT PROTOCOL
*   **Identity Preservation:** Respect existing project type if viable.
*   **PURPOSE PIVOT:** Re-imagine vague/weak repositories as professional tools.
*   **PROFESSIONAL ARCHIVAL:** Treat archived repos as "Retired Products"; elevate metadata.

### 6. CHAIN OF THOUGHT (CoT) PROTOCOL
Before execution, perform deep analysis:
1.  **Audit:** Analyze repo content and purpose.
2.  **Pivot/Archive Decision:** Rename if necessary (`Archived-...`).
3.  **Naming Strategy:** Apply `<Product>-<Function>-<Platform>-<Type>` formula.
4.  **Replication Protocol:** Draft AI Agent Directives (`AGENTS.md` or `<details>` block).
5.  **File Generation:** Plan content for all required files.
6.  **Final Polish:** Ensure all badges (`chirag127`, `flat-square`) and "Standard 11" compliance.
7.  **Strict Adherence:** `PROPOSED_README.md` must strictly follow `AGENTS.md` directives.

### 7. DYNAMIC URL & BADGE PROTOCOL
*   **Base URL:** `https://github.com/chirag127/<New-Repo-Name>`
*   **Badge URLs:** All Shields.io badges must point to the Base URL or specific workflows.
*   **Consistency:** Never use old repo names in links.

</details>

## Contributing

Contributions are welcome! Please read our [CONTRIBUTING.md](./.github/CONTRIBUTING.md) file for details on our code of conduct, and the process for submitting pull requests.

## License

This project is licensed under the CC BY-NC 4.0 License - see the [LICENSE](./LICENSE) file for details.
