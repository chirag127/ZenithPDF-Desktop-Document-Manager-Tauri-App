# ZenithPDF: Client-Side Document Management Desktop App

ZenithPDF is a high-performance, privacy-first desktop application built with Tauri and Vite, designed for seamless, client-side PDF document management. Edit, convert, merge, and secure your documents without ever leaving your local machine.

![ZenithPDF Logo](https://raw.githubusercontent.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/main/assets/logo.png)

---

## Status Badges

[![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/ci.yml?style=flat-square&logo=github)](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App?style=flat-square&logo=codecov)](https://codecov.io/github/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-6449FF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Tauri](https://img.shields.io/badge/Tauri-47A63F?style=flat-square&logo=tauri&logoColor=white)](https://tauri.app/)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-blue.svg?style=flat-square)](http://creativecommons.org/licenses/by-nc/4.0/)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App?style=flat-square&logo=github)](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/stargazers)

---

## ✨ Features

*   **Client-Side Processing:** All operations are performed locally, ensuring maximum privacy and security.
*   **Comprehensive Toolkit:** Edit text, images, annotations; convert between formats (PDF to DOCX, JPG to PDF, etc.); merge multiple PDFs; reorder pages.
*   **High Performance:** Built with Tauri and Vite for a fast, responsive, and native desktop experience.
*   **Modern UI:** Intuitive and user-friendly interface powered by Tailwind CSS.
*   **Privacy First:** No cloud uploads or data collection.
*   **Open Source:** Developed under an open-source license, fostering community collaboration.

---

## 🗺️ Architecture Overview

ZenithPDF employs a modern, client-side architecture focusing on performance and maintainability.

mermaid
graph TD
    A[User Interface (Vite + React/Vue)] --> B{Tauri Backend};
    B --> C[PDF Processing Logic (Rust)];
    B --> D[File System Access];
    A --> E(Client-Side Storage);
    C --> F(PDF Manipulation Libraries);


---

## 🤖 AI AGENT DIRECTIVES

<details>
<summary>Click to view AI Agent Directives</summary>

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
**Directives:** Detect the project type and apply the **Apex Toolchain**. This repository, `ZenithPDF-Client-Side-Document-Management-Desktop-App`, is a Desktop Application built with Tauri and TypeScript.

*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend)**
    *   **Stack:** **TypeScript 6.x** (Strict mode enforced). **Vite 7** (with Rolldown for enhanced bundling). **Tailwind CSS v4** (for utility-first styling). **Tauri v2.x** (for building native desktop applications).
    *   **UI Framework:** Assume **React 20.x** or **Vue 4.x** as the default, providing robust component-based UI development.
    *   **Linting & Formatting:** **Biome** (version 10.x) for maximum speed and comprehensive code quality checks.
    *   **Testing:** **Vitest 2.x** for unit and integration testing, providing fast, Vite-native test execution. **Playwright 2.x** for end-to-end testing across major browsers and native environments.
    *   **Architecture:** **Feature-Sliced Design (FSD)** principles are MANDATORY for organizing the frontend codebase. This ensures scalability and clear separation of concerns.
    *   **State Management:** Utilize **Signals** (standardized API, e.g., Preact Signals, SolidJS Signals) for efficient and reactive state management.

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Low Level) - *Not directly applicable but Rust runtime in Tauri backend leverages these principles.***
    *   **Stack:** Rust (Cargo) or Go (Modules).
    *   **Lint:** Clippy / GolangCI-Lint.
    *   **Architecture:** Hexagonal Architecture (Ports & Adapters).

*   **SECONDARY SCENARIO C: DATA / AI / SCRIPTS (Python) - *Not applicable.***
    *   **Stack:** uv (Manager), Ruff (Linter), Pytest (Test).
    *   **Architecture:** Modular Monolith or Microservices.

---

## 4. DEVELOPMENT STANDARDS & PRACTICES
*   **Code Quality:** Enforce **SOLID principles**, **DRY (Don't Repeat Yourself)**, and **YAGNI (You Ain't Gonna Need It)**.
*   **Version Control:** Git. Branching strategy: Gitflow (or simplified variations like GitHub Flow).
*   **Package Management:** npm/yarn/pnpm for frontend dependencies. Cargo for Rust backend dependencies.
*   **CI/CD:** GitHub Actions. Minimum requirement: Lint, Test, Build on Pull Request, Deploy on Merge to `main`/`master`.
*   **Documentation:** Comprehensive code comments, READMEs, and architecture diagrams. Use **Mermaid** or ASCII trees for diagrams.
*   **Security:** Regular dependency vulnerability scanning. Adhere to OWASP Top 10. Sanitize all inputs. **Client-side secrets management** requires careful consideration; avoid embedding sensitive keys directly.

---

## 5. AGENTS.MD VERIFICATION PROTOCOL
*   **Self-Correction:** Agents must self-verify their adherence to these directives by re-reading `AGENTS.md` before executing any action.
*   **Dynamic Adaptation:** If project context (e.g., language, framework) changes, agents must consult **Section 3** to select the correct Apex Toolchain and update their operational parameters.
*   **Error Handling:** All agent actions must include robust error handling and logging, failing gracefully and providing actionable feedback.

</details>

---

## 🚀 Getting Started

### Prerequisites

*   Node.js (LTS recommended)
*   Tauri CLI
*   Rust (for Tauri backend)

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App.git
    cd ZenithPDF-Client-Side-Document-Management-Desktop-App
    

2.  **Install Dependencies:**
    bash
    # Using npm (recommended)
    npm install

    # Or using yarn
    # yarn install

    # Or using pnpm
    # pnpm install
    

### Development Server

Run the app in development mode:

bash
# For Vite frontend development
npm run dev

# To build and run the Tauri desktop app
tauri dev


---

## 🛠️ Development Scripts

| Script        | Description                                      |
| :------------ | :----------------------------------------------- |
| `npm run dev` | Starts the Vite development server.              |
| `npm run build` | Builds the Vite frontend application.            |
| `npm run tauri dev` | Runs the Tauri development server.               |
| `npm run tauri build` | Builds the Tauri desktop application.            |
| `npm run lint`  | Runs Biome linter.                               |
| `npm run format`| Runs Biome formatter.                            |
| `npm run test`  | Runs Vitest unit and integration tests.          |
| `npm run e2e`   | Runs Playwright end-to-end tests.                |

---

## ⚖️ License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**.

See the [LICENSE](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/blob/main/LICENSE) file for more details.

---

## ⭐ Contributing

We welcome contributions! Please read our [CONTRIBUTING.md](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/blob/main/.github/CONTRIBUTING.md) guide for details on how to submit pull requests and report issues.

---

## 🛡️ Security

For security concerns, please refer to our [SECURITY.md](https://github.com/chirag127/ZenithPDF-Client-Side-Document-Management-Desktop-App/blob/main/.github/SECURITY.md) policy.

---

## 💖 Acknowledgements

*   **Tauri:** For enabling the creation of fast, secure, and native desktop applications.
*   **Vite:** For its blazing-fast development server and build capabilities.
*   **Tailwind CSS:** For its efficient utility-first CSS framework.
*   **Biome:** For maintaining code quality and developer productivity.
*   **Vitest & Playwright:** For ensuring robust testing coverage.

---

**Star ⭐ this Repo if you find it useful!**
