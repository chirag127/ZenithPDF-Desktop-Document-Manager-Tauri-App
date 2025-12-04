# ZenithPDF: Desktop Document Manager & Toolkit

<p align="center">
  <a href="https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App">
    <img src="https://raw.githubusercontent.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/main/.github/assets/logo.png" alt="ZenithPDF Logo" width="120">
  </a>
</p>

<h3 align="center">Your Secure, High-Performance, Client-Side PDF Workbench</h3>

<p align="center">
  <a href="https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/ci.yml?style=flat-square&logo=github&label=Build" alt="Build Status"></a>
  <a href="https://codecov.io/gh/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App"><img src="https://img.shields.io/codecov/c/github/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App?style=flat-square&logo=codecov&label=Coverage" alt="Code Coverage"></a>
  <a href="#"><img src="https://img.shields.io/badge/TypeScript-Strict-3178C6?style=flat-square&logo=typescript" alt="TypeScript"></a>
  <a href="https://tauri.app"><img src="https://img.shields.io/badge/Tauri-v2-FFC031?style=flat-square&logo=tauri" alt="Tauri"></a>
  <a href="https://vitejs.dev"><img src="https://img.shields.io/badge/Vite-v5-646CFF?style=flat-square&logo=vite" alt="Vite"></a>
  <a href="https://biomejs.dev/"><img src="https://img.shields.io/badge/Biome-Lint%20%26%20Format-8669F4?style=flat-square&logo=biome" alt="Biome Linter"></a>
  <a href="https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/blob/main/LICENSE"><img src="https://img.shields.io/github/license/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App?style=flat-square&label=License" alt="License"></a>
  <a href="https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/stargazers"><img src="https://img.shields.io/github/stars/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App?style=flat-square&logo=github&label=Stars" alt="GitHub Stars"></a>
</p>

<p align="center">
  <em>ZenithPDF is a high-performance, privacy-first desktop application for managing PDF documents entirely on your local machine. Built with Tauri v2, it provides a secure, client-side environment for editing, converting, merging, and splitting PDFs without ever uploading your files to the cloud.</em>
  <br><br>
  <a href="https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/stargazers"><strong>Star ⭐ this Repo</strong></a> to support its development!
</p>

---

## Table of Contents

- [✨ Features](#-features)
- [🏛️ Architecture](#️-architecture)
- [🤖 AI Agent Directives](#-ai-agent-directives)
- [🚀 Getting Started](#-getting-started)
- [🛠️ Development Scripts](#️-development-scripts)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

## ✨ Features

- **100% Client-Side:** Your files are never uploaded. All processing happens locally for maximum privacy.
- **PDF Conversion:** Convert documents to and from PDF format.
- **Document Editing:** Perform essential edits on PDF files.
- **Merge & Split:** Combine multiple PDFs into one or split a single PDF into several files.
- **Secure & Performant:** Built with Rust-powered Tauri backend for native performance and security.
- **Cross-Platform:** A single codebase delivers native applications for Windows, macOS, and Linux.

## 🏛️ Architecture

This project adheres to **Feature-Sliced Design (FSD)**, a scalable architectural methodology for frontend applications. This ensures a clear separation of concerns, enhances maintainability, and simplifies onboarding for new developers.

plaintext
src/
├── app/             # App-level logic, providers, routing
├── pages/           # Page components (e.g., EditorPage, MergerPage)
├── widgets/         # Composite UI blocks (e.g., FileDropzone, MainToolbar)
├── features/        # Business logic features (e.g., convert-pdf, merge-documents)
├── entities/        # Business entities (e.g., PDFDocument, AppSettings)
├── shared/          # Reusable modules, UI-kit, APIs, configs
└── src-tauri/       # Rust core for native OS interaction & high-performance tasks


## 🤖 AI Agent Directives

<details>
<summary><strong>SYSTEM: APEX TECHNICAL AUTHORITY (DECEMBER 2025)</strong></summary>

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. INPUT PROCESSING & COGNITION
- **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal user typos. You must **INFER** technical intent based on the project context.
- **Logic Anchor:** Treat this `README.md` as the **Single Source of Truth (SSOT)**.
- **Validation:** Use `docfork` to verify *every* external API signature. Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. CONTEXT-AWARE APEX TECH STACK (LATE 2025)
This project, `ZenithPDF-Desktop-Document-Manager-Tauri-App`, is a native desktop application.

- **PRIMARY SCENARIO: NATIVE DESKTOP APP (Tauri)**
    - **Stack:** This project is built on a modern **TypeScript** stack, leveraging **Vite** for the frontend build process and **Tauri v2** to create a native, cross-platform desktop application from a web-based UI. The Rust backend in `src-tauri` handles high-performance, secure file system operations.
    - **Linting & Formatting:** Utilizes **Biome** for unparalleled speed in linting, formatting, and code analysis, ensuring a consistent and high-quality codebase.
    - **Architecture:** Implements **Feature-Sliced Design (FSD)**. This strict, scalable architecture organizes code by business domain slices, promoting modularity, decoupling, and maintainability.
    - **Testing:** Employs **Vitest** for unit/integration tests and **Playwright** for robust end-to-end (E2E) testing of the application's user interface and native interactions.
    - **UI/UX:** Employs **TailwindCSS v4** for a utility-first styling approach, enabling rapid development of a clean and responsive user interface. State management is handled via modern patterns like **Signals**.

- **Verification Commands:**
    - `npm run lint`: Run Biome to check for linting and formatting errors.
    - `npm run test`: Execute unit and integration tests with Vitest.
    - `npm run test:e2e`: Run end-to-end tests with Playwright.
    - `npm run build`: Compile and build the native desktop application.

</details>

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18+)
- [Rust & Cargo](https://www.rust-lang.org/tools/install)
- System dependencies for Tauri (see [Tauri Docs](https://tauri.app/v1/guides/getting-started/prerequisites))

### Installation

1.  **Clone the repository:**
    sh
    git clone https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App.git
    cd ZenithPDF-Desktop-Document-Manager-Tauri-App
    

2.  **Install dependencies:**
    sh
    npm install
    

3.  **Run the development server:**
    sh
    npm run tauri dev
    

## 🛠️ Development Scripts

| Script          | Description                                           |
| --------------- | ----------------------------------------------------- |
| `tauri dev`     | Starts the development server with hot-reloading.     |
| `tauri build`   | Builds the production-ready native application.       |
| `lint`          | Lints and formats the codebase using Biome.           |
| `test`          | Runs unit and integration tests via Vitest.           |
| `test:e2e`      | Runs end-to-end tests via Playwright.                 |

## 🤝 Contributing

Contributions are welcome! Please read the [**CONTRIBUTING.md**](https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/blob/main/.github/CONTRIBUTING.md) guide for details on our code of conduct and the process for submitting pull requests.

For security-related concerns, please review our [**Security Policy**](https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/blob/main/.github/SECURITY.md).

## 📜 License

This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](https://github.com/chirag127/ZenithPDF-Desktop-Document-Manager-Tauri-App/blob/main/LICENSE).
