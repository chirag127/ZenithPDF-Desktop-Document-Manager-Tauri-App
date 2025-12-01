---
name: Bug Report
about: Report an issue with Zenith-PDF-Document-Management-Platform
title: "[BUG]: Short, descriptive title"
labels: ["bug", "triage"]
assignees: ""

---

## 🐛 Symptom Description

**BLUF (Bottom Line Up Front):** Describe the bug in one concise sentence.

--- 

### 🎯 Expected Behavior

What *should* have happened when you performed the action?

### 🛑 Actual Behavior

What *actually* happened? Include error messages, unexpected UI shifts, or incorrect outputs.

### 🔬 Steps to Reproduce

Provide a clear, numbered sequence of actions that reliably triggers this bug. **Zero ambiguity allowed.**

1.  Navigate to `/path/to/feature`.
2.  Ensure configuration XYZ is set.
3.  Click the [Action Button].
4.  Observe outcome Y.

### 🛠 Environment & Context

**This information is critical for debugging and adheres to the Apex Standard.**

*   **Platform:** (e.g., Desktop App via Tauri, Web Browser via Vite/SPA)
*   **OS & Version:** (e.g., macOS Sonoma 14.1, Windows 11 23H2)
*   **Browser (if applicable):** (e.g., Chrome 120.0, Firefox 119.0)
*   **Zenith PDF Version/Build Hash:** (If known, e.g., `v1.2.0-alpha.4` or `a3b1c9d`)
*   **Specific PDF Input:** (e.g., File size, content complexity, password protected? Attach sample if safe.)

### 🖼️ Visual Evidence

(Attach screenshots or screen recordings demonstrating the faulty state.)

### 💡 Proposed Fix (Optional)

If you have an idea for the solution, please describe it. We prioritize fixes that align with **SOLID principles** and **CQS separation**.

---

<details>
<summary>🤖 AI Agent Directive Context (LATE 2025 Standard)</summary>

**Project Stack Alignment:** TypeScript (Strict), Vite 7, Tauri v2.x, Biome, Vitest, Playwright.

**Architectural Focus:** Ensuring component isolation (FSD adherence), strict type safety, and performance compliance (INP < 200ms).

**Debugging Protocol:** Prioritize examining state management side-effects and asynchronous data flow logic (`Promise` chains or `Signals` updates) first. Run `biome check --error-on-warnings` locally before submission.
</details>