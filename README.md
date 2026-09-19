# VEXO — Community Link Directory & Discovery Platform

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Supabase](https://img.shields.io/badge/Backend-Supabase-3ECF8E?style=flat\&logo=supabase)](https://supabase.com)
[![HTML5](https://img.shields.io/badge/Built%20With-HTML%2FCSS%2FJS-E34F26?style=flat\&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/HTML)

As of **9/11/2026**, Vexo Proxy List has been released.

Today we also would like to say our prayers to help the people who were lost when the 9/11 attacks happened. May they rest in peace and find life in a new world.

VEXO is a community-driven web directory and discovery platform. Users can submit useful links, vote on submissions, bookmark favorites, interact through community tools, and use built-in utilities and AI-powered features — all supported by moderation and management tools.

---

## Features

### Link Management

* **Community Vault** — Browse approved community submissions with search, filtering, and categorization
* **Link Submission** — Submit links for moderation
* **Bulk Submission** — Submit multiple links using CSV-style entries
* **Approval Workflow** — Submissions start as `pending` until approved by administrators
* **Voting System** — Upvote/downvote links
* **Favorites** — Save links to your personal vault
* **View Tracking** — Track views on community links
* **Duplicate / Link Management** — Help keep the directory organized and useful

### Community Features

* **Authentication** — Email/password authentication through Supabase
* **Anonymous Submissions** — Submit links without an account using automatically generated anonymous IDs
* **Real-time Chat** — Community chat with profanity filtering and moderation support
* **Replies** — Reply to community messages
* **Profile Pictures** — Upload and manage profile pictures for chat
* **Customizable UI** — Neon Grid, Deep Space, and Clean visual modes
* **Accent Colors** — Customize the VEXO interface
* **Compact Mode** — Reduce spacing for a denser interface
* **Custom Cursor** — Neon cursor and cursor-ring effects
* **Click Effects** — Geometric shapes appear and fade around the pointer when clicking

### VEXO AI

* **VEXO AI** — Dedicated AI assistant integrated into the VEXO ecosystem
* **Separate AI Application** — VEXO AI runs as its own project while being integrated into VEXO Community
* **Ollama Cloud** — AI inference is handled through Ollama Cloud
* **GLM-5.3** — VEXO AI currently uses GLM-5.3 as its primary model
* **Supabase Edge Function** — Secure backend bridge between the VEXO AI frontend and Ollama
* **AI Chat Interface** — Send prompts and receive AI responses directly through VEXO

### Admin & Moderation

* **Admin Dashboard** — Centralized moderation and management interface
* **Moderation Queue** — Review, approve, and reject submitted links
* **Safety Scanning** — VirusTotal integration for threat intelligence checks
* **Uptime Monitoring** — Server-side checking of approved links
* **Broken Link Detection** — Detect unreachable or removed links
* **Link Removal** — Remove links identified as broken or unsafe
* **Takedown Requests** — Built-in DMCA/legal request workflow with status tracking
* **Announcements** — Publish prominent homepage announcements and changelogs
* **User Roles** — Admin roles and protected administration features
* **2FA Support** — TOTP-based two-factor authentication (**In Progress**)

### Built-in Toolbox

Client-side utilities that run directly in the browser:

* **Base64 Codec** — Encode and decode Base64
* **URL Codec** — Encode and decode URLs
* **JSON Formatter** — Format JSON data
* **Hash Generator** — SHA-1, SHA-256, and SHA-512
* **UUID Generator** — Generate UUIDs
* **Password Generator** — Configurable password length and symbols
* **Text Counter** — Characters, words, lines, and bytes
* **Timestamp Converter** — Convert Unix timestamps into readable dates
* **Color Converter** — HEX ↔ RGB conversion
* **Case Converter** — Uppercase, lowercase, title case, sentence case, camelCase, snake_case, and kebab-case
* **JavaScript Obfuscator** — Multi-layer JavaScript obfuscation with randomized transformations designed to make source analysis substantially harder

### Additional Tools

* **Web Proxy** — Embedded web browsing interface
* **File Sharing** — Integration with the VEXO File Sharing service
* **Terms of Use** — Legal information, disclaimers, and takedown request forms
* **Announcements System** — Homepage notices and changelog management
* **VEXO AI** — AI assistant available directly within the VEXO ecosystem

---

## Technology

VEXO is primarily built with:

* **HTML**
* **CSS**
* **JavaScript**
* **Supabase**
* **Supabase Edge Functions**
* **Ollama Cloud**
* **GLM-5.3**
* **GitHub Pages**
* **VirusTotal API**

The main VEXO interface is designed to remain lightweight and compatible with static GitHub Pages hosting while using Supabase for backend functionality.

---

## Project Structure

VEXO is separated into multiple projects and services that work together:

```text
VEXO Community
├── Community Vault
├── Community Chat
├── Admin Center
├── Toolbox
├── Web Proxy
├── File Sharing
└── VEXO AI
      ├── GitHub Pages frontend
      ├── Supabase Edge Function
      └── Ollama Cloud / GLM-5.3
```

---

## VEXO AI Architecture

VEXO AI is maintained separately from the main VEXO Community interface.

```text
VEXO Community
       │
       │ iframe
       ▼
    VEXO AI
       │
       │ HTTPS
       ▼
Supabase Edge Function
       │
       ▼
  Ollama Cloud
       │
       ▼
     GLM-5.3
```

This keeps the AI application separate from the main VEXO frontend while allowing it to be accessed directly inside VEXO Community.

---

## Hosting

The VEXO ecosystem is designed around GitHub Pages and Supabase.

```text
GitHub Pages
    │
    ├── VEXO Community
    └── VEXO AI
             │
             ▼
         Supabase
             │
             ▼
        Edge Functions
             │
             ▼
        External APIs
```

---

## License

This project is licensed under the **MIT License**.

See the [LICENSE](LICENSE) file for details.
