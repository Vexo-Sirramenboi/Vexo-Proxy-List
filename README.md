# VEXO — Community Link Directory & Discovery Platform

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Supabase](https://img.shields.io/badge/Backend-Supabase-3ECF8E?style=flat&logo=supabase)](https://supabase.com)
[![HTML5](https://img.shields.io/badge/Built%20With-HTML%2FCSS%2FJS-E34F26?style=flat&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/HTML)

VEXO is a community-driven web directory and discovery platform. Users can submit useful links, vote on submissions, bookmark favorites, and engage in real-time chat—all with robust moderation tools.

---

##  Features

###  Link Management
- **Community Vault** — Browse approved community submissions with search, filtering, and categorization
- **Link Submission** — Submit single links or bulk CSV-style entries for moderation
- **Approval Workflow** — Submissions start as "pending" until approved by administrators
- **Voting System** — Upvote/downvote links to surface quality content
- **Favorites** — Save links to your personal vault for quick access
- **View Tracking** — Automatic view counting per link

###  User Features
- **Authentication** — Email/password auth via Supabase with profile management
- **2FA Support** — TOTP-based two-factor authentication for enhanced security (In Progress)
- **Anonymous Submissions** — Submit links without an account (auto-generated anonymous IDs)
- **Real-time Chat** — Community live chat with profanity filtering and message moderation
- **Customizable UI** — Toggle between themes (Neon Grid, Deep Space, Clean), accent colors, compact mode, and cursor effects

###  Admin & Moderation
- **Admin Dashboard** — Comprehensive moderation queue with approval/rejection workflows
- **Safety Scanning** — VirusTotal integration for automated threat intelligence on submitted links
- **Uptime Monitoring** — Bulk HTTP status checking with automatic broken link detection/removal
- **Takedown Requests** — Built-in DMCA/legal request workflow with status tracking
- **Announcements** — Publish flashy homepage banners with changelog history
- **User Roles** — Admin role management with protected routes

###  Built-in Toolbox
Client-side utilities that run entirely in the browser:
- Base64 & URL codec (encode/decode)
- JSON Formatter
- Hash Generator (SHA-1, SHA-256, SHA-512)
- UUID Generator
- Password Generator (configurable length & symbols)
- Text Counter (characters, words, lines, bytes)
- Timestamp Converter
- Color Converter (HEX ↔ RGB)
- Case Converter (upper, lower, title, camelCase, snake_case, kebab-case)

###  Additional Tools
- **Web Proxy** — Embedded iframe proxy for browsing external sites
- **File Sharing** — Integration with external file sharing service
- **Terms of Use** — Auto-generated terms page with legal disclaimers and takedown forms
