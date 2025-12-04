# PDF-Spokable-AI-Transformer-Web-App

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/PDF-Spokable-AI-Transformer-Web-App/ci.yml?style=flat-square)](https://github.com/chirag127/PDF-Spokable-AI-Transformer-Web-App/actions/workflows/ci.yml)
[![Coverage](https://img.shields.io/codecov/c/github/chirag127/PDF-Spokable-AI-Transformer-Web-App?style=flat-square)](https://codecov.io/gh/chirag127/PDF-Spokable-AI-Transformer-Web-App)
[![Language](https://img.shields.io/github/languages/top/chirag127/PDF-Spokable-AI-Transformer-Web-App?style=flat-square)]()
[![License](https://img.shields.io/github/license/chirag127/PDF-Spokable-AI-Transformer-Web-App?style=flat-square)](https://github.com/chirag127/PDF-Spokable-AI-Transformer-Web-App/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/PDF-Spokable-AI-Transformer-Web-App?style=flat-square)](https://github.com/chirag127/PDF-Spokable-AI-Transformer-Web-App)

[⭐ Star this Repo ⭐](https://github.com/chirag127/PDF-Spokable-AI-Transformer-Web-App)

## 🚀 Project Overview

This repository houses a cutting-edge, client-side Web Application designed to transform static PDF documents into highly accessible, AI-optimized spoken content. It leverages advanced client-side parsing combined with the Gemini API for intelligent contextual extraction before utilizing native Web Speech Synthesis for flawless in-browser playback.

This solution prioritizes performance and user experience by minimizing server load and providing immediate, intelligent audio feedback directly within the browser environment.

## 🏗️ Architecture Overview (Late 2025 Standard)

This application adheres to a modern component-driven architecture, prioritizing granular separation of concerns (FSD principles adapted for Web Components) and leveraging WebAssembly/Web Workers for heavy PDF parsing tasks to maintain UI responsiveness.

mermaid
graph TD
    A[User Interface: React/Vite] --> B{PDF File Input};
    B --> C[Web Worker / WASM Parser];
    C -- Extracted Text Chunks --> D(Client-Side Pre-Processor);
    D -- Clean Context --> E[Gemini API Agent (Extraction/Summarization)];
    E -- Structured Audio Script --> F[Text-to-Speech (TTS) Engine - Web Speech API];
    F --> G[Playback Controller];
    G --> A;
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style E fill:#ccf,stroke:#333,stroke-width:2px


## 🧭 Table of Contents

1. [🚀 Project Overview](#-project-overview)
2. [🏗️ Architecture Overview (Late 2025 Standard)](#️-architecture-overview-late-2025-standard)
3. [🧭 Table of Contents](#-table-of-contents)
4. [✨ Key Features](#-key-features)
5. [🛠️ Apex Toolchain & Technology Stack](#️-apex-toolchain--technology-stack)
6. [🤖 AI Agent Directives (SSOT for Automation)](#-ai-agent-directives-ssot-for-automation)
7. [⚙️ Development & Setup](#-development--setup)
8. [📚 Licensing & Contribution](#-licensing--contribution)

## ✨ Key Features

*   **Intelligent Extraction:** Utilizes the Gemini API for semantic analysis of PDF content chunks, ensuring only relevant, contextually coherent text is sent for synthesis.
*   **Client-Side Focus:** Maximize browser performance; only AI calls leverage external services.
*   **Seamless Playback:** In-browser TTS with chapter/section seeking capabilities.
*   **Type Safety:** Built entirely in **TypeScript** ensuring robustness against runtime errors.
*   **Modern Tooling:** Powered by **Vite** for lightning-fast development cycles and **TailwindCSS** for utility-first styling.

## 🛠️ Apex Toolchain & Technology Stack

| Component | Technology | Version Standard | Rationale |
| :--- | :--- | :--- | :--- |
| **Language** | TypeScript | 6.x (Strict Mode) | Superior Type Safety & IDE Support. |
| **Build/Bundler** | Vite | 7.x | Zero-config, extreme speed via ESBuild integration. |
| **Styling** | TailwindCSS | v4 (Alpha/RC) | Utility-first, atomic styling system. |
| **Testing** | Vitest (Unit) / Playwright (E2E) | Latest | Fast in-memory unit testing; robust browser automation. |
| **AI Backend** | Google Gemini API | Pro/Flash Models | Contextual reasoning and high-quality text structuring. |
| **Architecture** | Feature-Sliced Design (FSD) Concepts | Adapted | Clear feature encapsulation and dependency management. |

## 🤖 AI Agent Directives (SSOT for Automation)

<details>
<summary>Click to view Architectural and Verification Directives (AGENTS.md Reference)</summary>

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
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context (`PDF-Spokable-AI-Transformer-Web-App`).
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs. Verify Gemini API endpoint signatures.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards** for Client-Side TTS best practices and **2026 UI Trends** (e.g., micro-interactions).
    *   **Validation:** Use `docfork` to verify *every* external API contract (especially Gemini).
    *   **Reasoning:** Engage `clear-thought-two` to architect complex asynchronous text processing flows *before* writing JavaScript/TypeScript.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** This repository is a **WEB / APP / GUI (Modern Frontend)** project.

*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend)**
    *   **Stack:** **TypeScript (Strict)**, **Vite 7**, **TailwindCSS v4**, **React 19/Signals**.
    *   **Lint/Test:** **Biome** (Speed) + **Vitest** (Unit) + **Playwright** (E2E).
    *   **Architecture:** **Feature-Sliced Design (FSD)** for component layering (layers: app, pages, features, entities, shared).
    *   **AI Integration:** Ensure all Gemini API calls are proxied through a secure `services/gemini-adapter` layer, handling streaming responses efficiently.

---

## 4. CORE ARCHITECTURAL MANDATES

*   **SOLID Principles:** Enforce Dependency Inversion (D) aggressively in the UI/Data layer separation.
*   **DRY:** Abstract all repetitive UI elements into shared components.
*   **YAGNI:** Do not over-engineer server endpoints; focus on client-side capability.
*   **SECURITY:** Never expose API keys client-side. Assume all external calls must be routed through a secure gateway (even if this repo is client-only, structure the code anticipating a proxied environment).

## 5. VERIFICATION COMMANDS

| Command | Tool | Purpose |
| :--- | :--- | :--- |
| `npm run lint` | Biome | Format and check code style compliance. |
| `npm run test:unit` | Vitest | Run fast unit tests across feature slices. |
| `npm run test:e2e` | Playwright | Validate complete user journeys (PDF upload to playback). |
| `npm run dev` | Vite | Start the optimized development server. |

</details>

## ⚙️ Development & Setup

Follow the Apex standard for environment readiness.

1.  **Clone Repository:**
    bash
    git clone https://github.com/chirag127/PDF-Spokable-AI-Transformer-Web-App.git
    cd PDF-Spokable-AI-Transformer-Web-App
    

2.  **Install Dependencies (Using uv/npm context):**
    Since this is a Web App, we rely on npm/yarn/pnpm for frontend tooling, managed by Vite/TypeScript.
    bash
    # Assuming npm is the package manager, aligning with TypeScript/Vite stack
    npm install
    

3.  **Environment Configuration:**
    Ensure your `.env` file contains the necessary API keys, securely managed (e.g., using Vite's environment variable handling):
    env
    VITE_GEMINI_API_KEY="YOUR_SECURE_KEY_HERE"
    

### Development Scripts

| Script | Command | Description |
| :--- | :--- | :--- |
| Start Dev Server | `npm run dev` | Launches the application with Hot Module Replacement (HMR). |
| Build Production | `npm run build` | Creates optimized, minified static assets. |
| Run Unit Tests | `npm run test:unit` | Executes Vitest suite. |
| Run E2E Tests | `npm run test:e2e` | Executes Playwright end-to-end scenarios. |
| Code Linting | `npm run lint` | Runs Biome for style and error checking. |

## 📚 Licensing & Contribution

This project is protected under the **Creative Commons Attribution-NonCommercial 4.0 International License**. See the [LICENSE](https://github.com/chirag127/PDF-Spokable-AI-Transformer-Web-App/blob/main/LICENSE) file for details.

We welcome contributions that adhere to the standards outlined in `.github/CONTRIBUTING.md`.
