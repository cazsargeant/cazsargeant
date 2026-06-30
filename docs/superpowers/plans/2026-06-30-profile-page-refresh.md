# Profile Page Refresh Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Rewrite the GitHub profile README so it positions Caz as a senior technical leader with platform/cloud depth and a practical AI enablement thread.

**Architecture:** Single-file GitHub profile README rewrite using GitHub-flavoured Markdown, lightweight HTML tables, and shields.io badges. The page relies on concise copy, spacing, and section hierarchy rather than unsupported GitHub CSS.

**Tech Stack:** Markdown, GitHub-compatible HTML tables, shields.io badges.

## Global Constraints

- Primary direction: Operator-Leader.
- Secondary thread: practical AI platform and enablement.
- Target reader: hiring or networking.
- Modify `README.md` only unless a real asset is added.
- Keep Markdown and HTML GitHub-compatible.
- Do not add claims about public repos that are not available yet.
- Keep the page readable even if shields.io badges fail to load.
- Do not include GitHub stats, streak widgets, trophy widgets, or a broken banner reference.

---

## File Structure

- Modify: `README.md` - complete profile page content.
- No new assets. A banner image should not be referenced until it exists.

## Task 1: Rewrite README Content

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: `docs/superpowers/specs/2026-06-30-profile-page-refresh-design.md`
- Produces: GitHub profile README with header, thesis, capability blocks, selected work, tools/credentials, sectors, and contact links.

- [ ] **Step 1: Replace README with the approved structure**

Use these exact sections in order:

```markdown
<div align="center">

# Hey, I'm Caz

**Technical leadership · Platform engineering · Cloud, security and AI adoption**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0072b1?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/cazsargeant)
[![Beyond](https://img.shields.io/badge/bynd.com-4285F4?logo=google-cloud&logoColor=white)](https://bynd.com)
![Manchester](https://img.shields.io/badge/Manchester-%F0%9F%93%8D-555)

</div>

---

<div align="center">

I lead cloud and platform work for organisations that need technology to become more reliable, secure and useful.

My background is hands-on engineering, but the work is usually bigger than infrastructure: shaping technical direction, helping teams adopt better practices, and turning cloud, security and AI ideas into systems people can actually run.

</div>

---

<table>
<tr>
<td width="33%" valign="top">

### Platform delivery

Designing and delivering cloud platforms, landing zones, migrations, serverless systems and Kubernetes foundations that teams can operate with confidence.

![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?logo=google-cloud&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-623CE4?logo=terraform&logoColor=white)

</td>
<td width="33%" valign="top">

### Technical leadership

Bridging strategy and delivery: shaping direction, making trade-offs clear, aligning stakeholders and helping engineering teams adopt better ways of working.

![Architecture](https://img.shields.io/badge/Architecture-555)
![DevSecOps](https://img.shields.io/badge/DevSecOps-3fb950)
![Delivery](https://img.shields.io/badge/Delivery_Leadership-f78166)

</td>
<td width="33%" valign="top">

### AI enablement

Helping teams use AI where it is genuinely useful: internal assistants, developer tooling, cloud-native AI services and secure adoption patterns.

![Gemini](https://img.shields.io/badge/Gemini-4285F4?logo=google-cloud&logoColor=white)
![AI Tooling](https://img.shields.io/badge/AI_Tooling-555)
![AI Security](https://img.shields.io/badge/AI_Security-8b5cf6)

</td>
</tr>
</table>

---

## Selected work
```

- [ ] **Step 2: Add selected work entries**

Include the five current examples with outcome-led copy:

```markdown
## Selected work

**Serverless Data Pipeline - Public Sector** &nbsp; ![in progress](https://img.shields.io/badge/status-in_progress-blue)

Shaping a secure, serverless data processing platform for financial statistics across public sector departments, with governance and operational reliability designed in from the start.

![Cloud Run](https://img.shields.io/badge/Cloud_Run-4285F4?logo=google-cloud&logoColor=white)
![Cloud Functions](https://img.shields.io/badge/Cloud_Functions-4285F4?logo=google-cloud&logoColor=white)
![DevSecOps](https://img.shields.io/badge/DevSecOps-3fb950)

<br>

**PSA Platform - Professional Services Firm** &nbsp; ![done](https://img.shields.io/badge/status-done-brightgreen)

Delivered a full-stack internal platform for staff allocation, project delivery and billing, adding AI-powered insight and workflows that improved operational visibility.

![Terraform](https://img.shields.io/badge/Terraform-623CE4?logo=terraform&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?logo=google-cloud&logoColor=white)

<br>

**Secure Landing Zone - Formula E Trackside Analytics** &nbsp; ![done](https://img.shields.io/badge/status-done-brightgreen)

Designed a GCP landing zone for real-time trackside analytics, integrating BigQuery and Gemini while enabling the engineering team to operate the platform independently.

![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?logo=google-cloud&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?logo=googlebigquery&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?logo=google-cloud&logoColor=white)

<br>

**Regulated Data Centre Exit - Major UK Bank** &nbsp; ![done](https://img.shields.io/badge/status-done-brightgreen)

Helped deliver a regulated migration from on-premise systems to GCE and Kubernetes, covering HA/DR design, legacy application re-architecture and CI/CD foundations.

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![Cloud Build](https://img.shields.io/badge/Cloud_Build-4285F4?logo=google-cloud&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white)

<br>

**AI Chat Assistant - UK Water Company** &nbsp; ![done](https://img.shields.io/badge/status-done-brightgreen)

Built the cloud platform foundations for a custom Gemini assistant on Cloud Run, helping staff query internal documentation and content through a governed interface.

![Cloud Run](https://img.shields.io/badge/Cloud_Run-4285F4?logo=google-cloud&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?logo=google-cloud&logoColor=white)
```

- [ ] **Step 3: Keep future pinned repo guidance out of README copy**

Do not add a reference projects section to `README.md`.

Keep future pin ideas as implementation guidance only:

- Wiz + Terraform security posture demo
- Secure Kubernetes platform demo
- Gemini or AI assistant reference build
- Serverless data pipeline pattern
- Cloud landing zone starter
- AI developer productivity tooling

- [ ] **Step 4: Add tools, credentials, sectors and contact close**

Group badges below the story:

```markdown
---

## Tools and credentials

![Professional Cloud Architect](https://img.shields.io/badge/Professional_Cloud_Architect-4285F4?logo=google-cloud&logoColor=white)
![Professional DevOps Engineer](https://img.shields.io/badge/Professional_DevOps_Engineer-4285F4?logo=google-cloud&logoColor=white)
![Professional Network Engineer](https://img.shields.io/badge/Professional_Network_Engineer-4285F4?logo=google-cloud&logoColor=white)
![GenAI Leader](https://img.shields.io/badge/GenAI_Leader-4285F4?logo=google-cloud&logoColor=white)

![Wiz Champion](https://img.shields.io/badge/Wiz_Champion-FF6B35)
![Wiz Cloud Security](https://img.shields.io/badge/Wiz_Cloud_Security-FF6B35)
![Security Strategy](https://img.shields.io/badge/Security_Strategy-f78166)

---

## Sectors

![Public Sector](https://img.shields.io/badge/Public_Sector-1d4ed8)
![Financial Services](https://img.shields.io/badge/Financial_Services-0ea5e9)
![Logistics](https://img.shields.io/badge/Logistics-f59e0b)
![Retail](https://img.shields.io/badge/Retail-ec4899)
![Startups](https://img.shields.io/badge/Startups-3fb950)
![Higher Education](https://img.shields.io/badge/Higher_Education-555)

---

<div align="center">

Open to conversations about platform leadership, cloud delivery, secure foundations and practical AI adoption.

[LinkedIn](https://www.linkedin.com/in/cazsargeant) · [Beyond](https://bynd.com)

</div>
```

- [ ] **Step 5: Verify Markdown constraints**

Run:

```bash
git diff --check
rg -n "banner\\.png|GitHub stats|streak|trophy|TODO|TBD" README.md
sed -n '1,260p' README.md
```

Expected:

- `git diff --check` exits with no output.
- `rg` only exits non-zero because there are no matches.
- `README.md` has no broken banner reference, TODO, TBD, or vanity widgets.

- [ ] **Step 6: Commit**

Run:

```bash
git add README.md
git commit -m "feat: refresh profile README positioning"
```
