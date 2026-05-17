---
name: profile-readme-redesign
description: Full redesign of cazsargeant GitHub profile README — dark premium aesthetic, Foundations/Frontier structure, project highlights
metadata:
  type: project
---

# GitHub Profile README Redesign

## Goals

- Impress potential employers and clients at a glance
- Reflect personal brand: stylish but nerdy, solid engineer with an eye on AI and security
- Distinct voice — not derivative of any colleague's profile
- Dark premium aesthetic inspired by windagency, but with original structure and copy

---

## Structure (top to bottom)

### 1. Banner image
- Full-width image at the top of the README
- File committed to repo root as `banner.png` (or similar), referenced with relative path: `![Banner](./banner.png)`
- User to generate: dark, premium, 1280×640px — suggested prompt: "dark cinematic tech banner, cloud infrastructure, abstract, 1280x640"

### 2. Header
- Centred
- Name: `Hey, I'm Caz 👋`
- Subtitle: `Platform Engineering Consultant · Beyond · Google Cloud Premier Partner`
  - "Beyond" coloured `#4285F4` (GCP blue)
- Three badges (default shields.io style — rounded, gradient depth):
  - LinkedIn → `https://img.shields.io/badge/LinkedIn-0072b1?logo=linkedin&logoColor=white`
  - Beyond website → `https://img.shields.io/badge/bynd.com-4285F4?logo=google-cloud&logoColor=white` (linked to https://bynd.com)
  - Manchester → `https://img.shields.io/badge/Manchester-📍-555`

### 3. Horizontal rule

### 4. Intro paragraph
Centred, max-width constrained, slightly lighter text:

> I help organisations get serious about cloud. That means architecture, infrastructure, platform work — but also the systems, processes and team enablement that make it stick.

### 5. Horizontal rule

### 6. Foundations / Frontier panels (2-column grid)

**⚡ FOUNDATIONS** (heading colour: `#3fb950`)
- Description: "Cloud infrastructure and platform engineering across large enterprise at Beyond. Designing, building and operating at scale."
- Badges (default shields.io style):
  - Google Cloud `#4285F4` `logo=google-cloud`
  - Kubernetes `#326CE5` `logo=kubernetes`
  - Terraform `#623CE4` `logo=terraform`
  - Docker `#2496ED` `logo=docker`
  - Firebase `#FFCA28` `logo=firebase`
  - Linux `#FCC624` `logo=linux`
  - Architecture `#555` (no logo)
  - DevSecOps `#3fb950` (no logo)
  - Security Strategy `#f78166` (no logo)

**🔭 FRONTIER** (heading colour: `#f78166`)
- Description: "Building at the intersection of AI and security — tooling strategy, cloud security posture, and exploring what intelligent systems change about how we build."
- Badges:
  - Wiz Champion `#FF6B35` (no logo)
  - AI Dev Tooling `#555` (no logo)
  - GCP GenAI Leader `#4285F4` `logo=google-cloud`
  - AI Security `#8b5cf6` (no logo)

### 7. Google Cloud Certifications
Section heading: `☁️ Google Cloud Certifications`
- Professional Cloud Architect `#4285F4` `logo=google-cloud`
- Professional DevOps Engineer `#4285F4` `logo=google-cloud`
- Professional Network Engineer `#4285F4` `logo=google-cloud`
- GenAI Leader `#4285F4` `logo=google-cloud`

### 8. Sectors
Section heading: `🏢 Sectors`
Text-only badges (no logos):
- Public Sector `#1d4ed8`
- Financial Services `#0ea5e9`
- Logistics `#f59e0b`
- Retail `#ec4899`
- Startups `#3fb950`

### 9. Selected work
Section heading: `🛠️ Selected work`

Each entry is a card with: coloured left border, title + status tag, description, tech badges.

Status tags:
- `in progress` — blue (`#1d3a6e` bg, `#93c5fd` text)
- `done` — green (`#1a3a2a` bg, `#6ee7a0` text)

| Project | Status | Left border | Description | Badges |
|---|---|---|---|---|
| Serverless Data Pipeline — Public Sector | in progress | `#4285F4` | Secure, serverless data processing platform handling financial statistics across multiple government departments. Security and data governance central to the architecture. | Cloud Run, Cloud Functions, DevSecOps |
| PSA Platform — Professional Services Firm | done | `#3fb950` | Full-stack internal platform for staff allocation, project delivery and billing with AI-powered insight. Delivered **£2M in operational savings**. | Terraform, Firebase, Gemini |
| Secure Landing Zone — Formula E Trackside Analytics | done | `#f78166` | GCP landing zone for real-time trackside analytics for an electric racing team. Integrated BigQuery and Gemini AI for data analysis. Trained the engineering team to operate independently. | Google Cloud, BigQuery, Gemini |
| Regulated Data Centre Exit — Major UK Bank | done | `#0ea5e9` | Rapid migration of on-prem applications to GCE and Kubernetes to meet end-of-life regulatory requirements. Delivered HA/DR architecture, rearchitected legacy systems, and built CI/CD pipelines. | Kubernetes, Cloud Build, Ansible |
| AI Chat Assistant — UK Water Company | done | `#8b5cf6` | Cloud platform infrastructure for a custom Gemini API on Cloud Run, enabling staff to query internal documentation and marketing content. | Cloud Run, Gemini |

---

## Design decisions

- **No vanity widgets** (GitHub stats, streak counter) — real project work tells a stronger story
- **Logos only on actual products used** — no logos on practices (Architecture, DevSecOps, Security Strategy), Wiz (not on shields.io), or sectors
- **Default shields.io badge style** — rounded corners, gradient depth (no `style=flat-square`)
- **Frontend stack omitted** — profile positions as infra/cloud/security/AI engineer; dev skills visible through project descriptions
- **"Beyond" appears once** in subtitle text; badge shows `bynd.com` only to avoid repetition
- **Banner image** not committed yet — placeholder in README until user generates and adds the file

---

## Files to create/modify

- `README.md` — full rewrite
- `banner.png` — user to provide; referenced from README
- `.gitignore` — add `.superpowers/` if not already present
