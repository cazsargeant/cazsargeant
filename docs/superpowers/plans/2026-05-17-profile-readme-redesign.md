# Profile README Redesign — Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Rewrite cazsargeant/cazsargeant README.md as a dark-aesthetic, professional profile with Foundations/Frontier panels, selected project highlights, and a banner image placeholder.

**Architecture:** Single README.md rewrite using GitHub-compatible HTML + Markdown. Two-column layout via HTML table (GitHub strips inline CSS so card backgrounds and coloured borders from the mockup are replaced by GitHub's default table rendering — all badges, copy and structure are preserved). Shields.io badges for all visual pills.

**Tech Stack:** Markdown, HTML (GitHub-flavoured), shields.io badges

---

## Files

- Modify: `README.md` — full rewrite
- Modify: `.gitignore` — add `.superpowers/`

---

## Task 1: Update .gitignore

**Files:**
- Modify: `.gitignore`

- [ ] **Step 1: Check if .gitignore exists**

```bash
cat .gitignore 2>/dev/null || echo "no .gitignore"
```

- [ ] **Step 2: Add .superpowers/ entry**

If `.gitignore` exists, append to it. If not, create it.

```bash
echo ".superpowers/" >> .gitignore
```

- [ ] **Step 3: Verify**

```bash
cat .gitignore
```

Expected: `.superpowers/` appears in the file.

- [ ] **Step 4: Commit**

```bash
git add .gitignore
git commit -m "chore: ignore .superpowers brainstorm directory"
```

---

## Task 2: Header — banner, name, subtitle, badges

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Replace README contents with header section**

Write the following as the entire contents of `README.md` (subsequent tasks will append):

```markdown
<div align="center">

![Banner](./banner.png)

# Hey, I'm Caz 👋

**Platform Engineering Consultant · [Beyond](https://bynd.com) · Google Cloud Premier Partner**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0072b1?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/cazsargeant)
[![Beyond](https://img.shields.io/badge/bynd.com-4285F4?logo=google-cloud&logoColor=white)](https://bynd.com)
![Manchester](https://img.shields.io/badge/Manchester-%F0%9F%93%8D-555)

</div>
```

- [ ] **Step 2: Preview in VS Code**

Open the markdown preview (Cmd+Shift+V). Verify:
- Banner shows a broken image placeholder (expected — file not committed yet)
- Name renders as H1
- Subtitle is bold with Beyond as a link
- Three badges appear on one line, centred

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add profile header with banner placeholder and badges"
```

---

## Task 3: Intro paragraph + horizontal rules

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append intro section**

Append to `README.md`:

```markdown

---

<div align="center">

I help organisations get serious about cloud. That means architecture, infrastructure, platform work — but also the systems, processes and team enablement that make it stick.

</div>

---
```

- [ ] **Step 2: Preview**

Verify the intro paragraph is centred, with horizontal rules above and below.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add intro paragraph"
```

---

## Task 4: Foundations / Frontier two-column panels

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append Foundations/Frontier section**

Append to `README.md`:

```markdown

<table>
<tr>
<td width="50%" valign="top">

**⚡ FOUNDATIONS**

Cloud infrastructure and platform engineering across large enterprise at [Beyond](https://bynd.com). Designing, building and operating at scale.

![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?logo=google-cloud&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-623CE4?logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![Architecture](https://img.shields.io/badge/Architecture-555)
![DevSecOps](https://img.shields.io/badge/DevSecOps-3fb950)
![Security Strategy](https://img.shields.io/badge/Security_Strategy-f78166)

</td>
<td width="50%" valign="top">

**🔭 FRONTIER**

Building at the intersection of AI and security — tooling strategy, cloud security posture, and exploring what intelligent systems change about how we build.

![Wiz Champion](https://img.shields.io/badge/Wiz_Champion-FF6B35)
![AI Dev Tooling](https://img.shields.io/badge/AI_Dev_Tooling-555)
![GCP GenAI Leader](https://img.shields.io/badge/GCP_GenAI_Leader-4285F4?logo=google-cloud&logoColor=white)
![AI Security](https://img.shields.io/badge/AI_Security-8b5cf6)

</td>
</tr>
</table>
```

- [ ] **Step 2: Preview**

Verify:
- Two columns side by side
- FOUNDATIONS left, FRONTIER right
- Badges wrap naturally within each column
- Descriptions readable

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add Foundations and Frontier panels"
```

---

## Task 5: Google Cloud Certifications + Sectors

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append Certifications and Sectors sections**

Append to `README.md`:

```markdown

---

### ☁️ Google Cloud Certifications

![Professional Cloud Architect](https://img.shields.io/badge/Professional_Cloud_Architect-4285F4?logo=google-cloud&logoColor=white)
![Professional DevOps Engineer](https://img.shields.io/badge/Professional_DevOps_Engineer-4285F4?logo=google-cloud&logoColor=white)
![Professional Network Engineer](https://img.shields.io/badge/Professional_Network_Engineer-4285F4?logo=google-cloud&logoColor=white)
![GenAI Leader](https://img.shields.io/badge/GenAI_Leader-4285F4?logo=google-cloud&logoColor=white)

---

### 🏢 Sectors

![Public Sector](https://img.shields.io/badge/Public_Sector-1d4ed8)
![Financial Services](https://img.shields.io/badge/Financial_Services-0ea5e9)
![Logistics](https://img.shields.io/badge/Logistics-f59e0b)
![Retail](https://img.shields.io/badge/Retail-ec4899)
![Startups](https://img.shields.io/badge/Startups-3fb950)
```

- [ ] **Step 2: Preview**

Verify:
- Certifications heading includes ☁️ emoji
- All 4 GCP cert badges appear in GCP blue
- Sectors badges appear in their distinct colours

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add Google Cloud certifications and sectors"
```

---

## Task 6: Selected work

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append Selected Work section**

Append to `README.md`:

```markdown

---

### 🛠️ Selected work

**Serverless Data Pipeline — Public Sector** &nbsp; ![in progress](https://img.shields.io/badge/status-in%20progress-blue)

Secure, serverless data processing platform handling financial statistics across multiple government departments. Security and data governance central to the architecture.

![Cloud Run](https://img.shields.io/badge/Cloud_Run-4285F4?logo=google-cloud&logoColor=white)
![Cloud Functions](https://img.shields.io/badge/Cloud_Functions-4285F4?logo=google-cloud&logoColor=white)
![DevSecOps](https://img.shields.io/badge/DevSecOps-3fb950)

<br>

**PSA Platform — Professional Services Firm** &nbsp; ![done](https://img.shields.io/badge/status-done-brightgreen)

Full-stack internal platform for staff allocation, project delivery and billing with AI-powered insight. Delivered **£2M in operational savings**.

![Terraform](https://img.shields.io/badge/Terraform-623CE4?logo=terraform&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?logo=google-cloud&logoColor=white)

<br>

**Secure Landing Zone — Formula E Trackside Analytics** &nbsp; ![done](https://img.shields.io/badge/status-done-brightgreen)

GCP landing zone for real-time trackside analytics for an electric racing team. Integrated BigQuery and Gemini AI for data analysis. Trained the engineering team to operate independently.

![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?logo=google-cloud&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?logo=googlebigquery&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?logo=google-cloud&logoColor=white)

<br>

**Regulated Data Centre Exit — Major UK Bank** &nbsp; ![done](https://img.shields.io/badge/status-done-brightgreen)

Rapid migration of on-prem applications to GCE and Kubernetes to meet end-of-life regulatory requirements. Delivered HA/DR architecture, rearchitected legacy systems, and built CI/CD pipelines.

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![Cloud Build](https://img.shields.io/badge/Cloud_Build-4285F4?logo=google-cloud&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white)

<br>

**AI Chat Assistant — UK Water Company** &nbsp; ![done](https://img.shields.io/badge/status-done-brightgreen)

Cloud platform infrastructure for a custom Gemini API on Cloud Run, enabling staff to query internal documentation and marketing content.

![Cloud Run](https://img.shields.io/badge/Cloud_Run-4285F4?logo=google-cloud&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?logo=google-cloud&logoColor=white)
```

- [ ] **Step 2: Preview**

Verify:
- Section heading shows 🛠️
- Each project has title (bold) + status badge on the same line
- "in progress" badge is blue, all "done" badges are green
- Tech badges appear below each description
- `<br>` spacers add visual separation between projects
- **£2M** renders in bold

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add selected work project highlights"
```

---

## Task 7: Add banner placeholder + final review

**Files:**
- Modify: `README.md` (add comment), optionally add `banner.png`

- [ ] **Step 1: Add banner placeholder comment at top of README**

Insert an HTML comment at the very top of `README.md` (above the `<div align="center">` block) as a reminder:

```markdown
<!-- Replace banner.png with your generated dark banner image (1280x640px recommended) before sharing -->
```

- [ ] **Step 2: Full end-to-end preview**

Open VS Code markdown preview and scroll through the full README. Check:
- [ ] Banner placeholder shows (broken image is expected)
- [ ] Header is centred with correct subtitle and 3 badges
- [ ] Intro paragraph is centred
- [ ] Two columns render for Foundations/Frontier
- [ ] All badges in Foundations have correct colours and logos
- [ ] All badges in Frontier have correct colours (no logos on Wiz, AI Dev Tooling, AI Security)
- [ ] Google Cloud Certifications heading includes ☁️
- [ ] All 4 cert badges are GCP blue with Google Cloud logo
- [ ] Sectors section shows 5 coloured text-only badges
- [ ] Selected work has 5 projects
- [ ] Serverless Pipeline has blue "in progress" badge
- [ ] Remaining 4 projects have green "done" badges
- [ ] £2M is bold in PSA project

- [ ] **Step 3: Push and verify on GitHub**

```bash
git push origin main
```

Open `https://github.com/cazsargeant` in a browser and verify the live profile renders correctly.

- [ ] **Step 4: Add banner image (when ready)**

When you have your banner image file:

```bash
cp /path/to/your/banner.png /Users/caz.sargeant/git-profile-readme/cazsargeant/banner.png
git add banner.png
git commit -m "feat: add profile banner image"
git push origin main
```

- [ ] **Step 5: Final commit if any tweaks made**

```bash
git add README.md
git commit -m "chore: final profile README polish"
git push origin main
```

---

## Notes

- GitHub strips inline CSS styles — the coloured card backgrounds and left borders from the mockup are not possible in a GitHub README. The design intent is preserved via badge colours, section structure, and copy.
- The Manchester badge uses URL-encoded emoji (`%F0%9F%93%8D` = 📍). If the badge doesn't render, fall back to plain text: `![Manchester](https://img.shields.io/badge/Manchester-UK-555)`
- The banner image is not included in this plan — generate it separately (Midjourney, Ideogram, or similar) using a prompt like: *"dark cinematic tech banner, abstract cloud infrastructure, blue and teal glows, 1280x640, no text"*
