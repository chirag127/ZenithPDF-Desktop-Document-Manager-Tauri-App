# 💎 ZenithPDF-Document-Management-Desktop-App

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/ZenithPDF-Document-Management-Desktop-App/ci.yml?style=flat-square&logo=github)](https://github.com/chirag127/ZenithPDF-Document-Management-Desktop-App/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/ZenithPDF-Document-Management-Desktop-App?style=flat-square)](https://codecov.io/gh/chirag127/ZenithPDF-Document-Management-Desktop-App)
[![Language](https://img.shields.io/github/languages/top/chirag127/ZenithPDF-Document-Management-Desktop-App?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![License](https://img.shields.io/github/license/chirag127/ZenithPDF-Document-Management-Desktop-App?style=flat-square&color=brightgreen)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/ZenithPDF-Document-Management-Desktop-App?style=flat-square&logo=github)](https://github.com/chirag127/ZenithPDF-Document-Management-Desktop-App)

**Star ⭐ this Repo if you find it useful!**

---

ZenithPDF is a high-performance, zero-dependency desktop application designed for comprehensive client-side PDF manipulation. Built using the modern **Tauri v2** framework, it delivers native performance while ensuring absolute data privacy by processing all files locally.

This repository embodies the **Apex Standard** for desktop application development, focusing on rigorous TypeScript typing, modular architecture, and exceptional user experience.

## 🏛️ Architecture Overview

The application adheres to a strict **Feature-Sliced Design (FSD)** paradigm, separating the application into distinct, independent layers to maximize maintainability and scalability.

mermaid
graph TD
    subgraph Frontend [Renderer Process (Vite/React)]
        UI(User Interface/Components)
        STATE(State Management/Signals)
    end

    subgraph Backend [Tauri Rust Core]
        INVOKE(IPC Invoker)
        FS(File System & OS Access)
        PDF_CORE(PDF Engine: PDF.js/PDFKit Adapter)
    end

    subgraph Feature Slices
        FEATURES(Features: Edit, Convert, Secure)
        UTILS(Shared Utilities)
    end

    UI --> STATE
    UI -- Invoke/Handle --> INVOKE
    INVOKE -- Bridge --> FS
    INVOKE -- Bridge --> PDF_CORE

    FEATURES --> UI
    FEATURES --> UTILS

    PDF_CORE -- Low-Level Ops --> FS

    classDef apex fill:#4a90e2,stroke:#333,stroke-width:2px,color:#fff;
    class UI,STATE,INVOKE,FS,PDF_CORE,FEATURES,UTILS apex;


## 📋 Table of Contents

1. [💎 ZenithPDF-Document-Management-Desktop-App](#-zenithpdf-document-management-desktop-app)
2. [🏛️ Architecture Overview](#️-architecture-overview)
3. [📋 Table of Contents](#-table-of-contents)
4. [🚀 Key Features](#-key-features)
5. [🤖 AI Agent Directives (Apex Standard)](#-ai-agent-directives-apex-standard)
6. [🛠️ Development & Setup](#-development--setup)
7. [📜 License](#-license)

## 🚀 Key Features

*   **High-Fidelity PDF Editing:** Inline text modification, annotation support, and layout adjustments.
*   **Universal Conversion:** Convert PDFs to standard image formats (PNG, JPEG) and document formats (DOCX, TXT) locally.
*   **Security & Privacy:** Client-side encryption/decryption and password protection leveraging Rust's secure primitives.
*   **Batch Processing:** Efficiently handle merges, splits, and compressions for large document sets.
*   **Native Performance:** Built with Tauri and Rust for near-native speed and minimal resource consumption.

## 🤖 AI Agent Directives (Apex Standard)

<details>
<summary>Click to view Apex Architecture & Verification Commands</summary>

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
    *   **No Guessing:** Do not hallucinate APIs. Do not rely on deprecated libraries.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends** specifically related to **Tauri/TypeScript Desktop Apps**.
    *   **Validation:** Use `docfork` to verify *every* external API signature, especially Tauri commands.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex inter-process communication (IPC) flows *before* writing Rust/TS bindings.

--- 

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** This repository, `ZenithPDF-Document-Management-Desktop-App`, is a **Web/App/GUI** project.

*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend)**
    *   **Stack:** **TypeScript 6.x (Strict, utilizing Node/TS compiler flags at level 90+)**, **Vite 7** (build optimization), **TailwindCSS v4** (utility-first styling), and **Tauri v2.x** (Desktop host).
    *   **Lint/Test:** **Biome** (Lint/Format Speed) + **Vitest** (Unit Testing) + **Playwright** (E2E Testing for UI flows).
    *   **Architecture:** Adheres strictly to **Feature-Sliced Design (FSD)**, ensuring that Presentation, Features, Entities, and Shared layers are mutually exclusive and maintain explicit dependencies.


## 4. ARCHITECTURAL MANDATES
1.  **SOLID Adherence:** Interfaces must be clearly separated (Interface Segregation Principle). State mutation must be centralized (Single Responsibility Principle).
2.  **DRY Principle Enforcement:** Custom PDF handling logic must be abstracted into isolated Rust sidecars accessible via Tauri IPC, preventing duplication in TypeScript logic.
3.  **YAGNI/KISS:** Maintain minimal dependencies. Only use dependencies that are essential for PDF rendering or OS interaction (e.g., `tauri-plugin-fs`, `pdfjs-dist` compatibility layer).
4.  **Security:** All IPC communication channels must be strongly typed and validated on the Rust side to prevent injection attacks from the renderer.

## 5. VERIFICATION COMMANDS (Run from root directory)
*   **Build & Lint Check (Fast Check):**
    bash
    npm run lint
    npm run test:unit
    
*   **Full CI Simulation (Includes E2E):**
    bash
    npm run ci:verify
    
*   **Tauri Native Build Check:**
    bash
    cargo check --workspace
    
</details>

## 🛠️ Development & Setup

This project requires Node.js (v20+ recommended), Rust, and the Tauri CLI prerequisites.

### Prerequisites
1.  Install Node.js and Rust.
2.  Ensure Cargo is installed via `rustup`.

### Installation
bash
git clone https://github.com/chirag127/ZenithPDF-Document-Management-Desktop-App.git
cd ZenithPDF-Document-Management-Desktop-App

# Use uv for blazing fast dependency resolution (2026 Standard)
npm install

# (Note: Rust dependencies for Tauri are managed via Cargo, check Cargo.toml)


### Development Commands
| Command | Description | Standard | 
| :--- | :--- | :--- | 
| `npm run dev` | Start the Vite development server with Tauri hot reloading. | Local Dev | 
| `npm run build` | Compiles the application for production release. | Build | 
| `npm run test:unit` | Runs all Jest/Vitest unit tests across TS modules. | Test | 
| `npm run test:e2e` | Executes end-to-end validation using Playwright. | Test | 
| `npm run format` | Applies Biome formatting rules across the codebase. | Lint/Style |

## 📜 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**. See the [LICENSE](LICENSE) file for details.
