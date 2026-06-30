---
name: profile-page-refresh
description: Refresh the cazsargeant GitHub profile README around technical leadership, platform delivery, and practical AI enablement.
metadata:
  type: project
---

# GitHub Profile Page Refresh

## Goal

Refresh the GitHub profile README so it reads as a senior technical leadership profile, not a generic cloud consultancy brochure. The page should make Caz look credible for broad technical leadership, with strong platform/cloud depth and a measured AI enablement thread.

The target reader is hiring or networking: someone deciding whether Caz is a serious technical leader who can shape direction, own delivery, and help teams adopt cloud, security, and AI practices that actually work.

## Positioning

Primary direction: Operator-Leader.

Secondary thread: practical AI platform and enablement.

The profile should communicate:

> Caz is a technical leader who makes cloud and platform work real inside organisations, with enough AI fluency to help teams adopt it responsibly rather than chase hype.

The voice should be direct, senior, practical, and specific. Avoid over-polished sales language, vanity widgets, and excessive badge walls.

## Page Structure

### 1. Header

Use a clean centred header:

```markdown
# Hey, I'm Caz

Technical leadership · Platform engineering · Cloud, security and AI adoption
```

Keep LinkedIn, Beyond, and Manchester badges, but keep the header visually quieter than the current version.

### 2. Opening Thesis

Use two short paragraphs:

```markdown
I lead cloud and platform work for organisations that need technology to become more reliable, secure and useful.

My background is hands-on engineering, but the work is usually bigger than infrastructure: shaping technical direction, helping teams adopt better practices, and turning cloud, security and AI ideas into systems people can actually run.
```

### 3. Capability Blocks

Replace the current Foundations / Frontier split with three clearer blocks:

- Platform delivery: GCP, Kubernetes, Terraform, serverless, migration, reliability, operating at scale.
- Technical leadership: strategy, advisory, enablement, stakeholder translation, delivery ownership, team practices.
- AI enablement: Gemini, AI tooling, secure adoption, internal assistants, developer productivity.

These should be short, tidy, and readable. Use a table for GitHub-compatible layout, but keep each cell concise.

### 4. Selected Work

Keep the selected work section, but rewrite descriptions around leadership and outcomes. Use verbs like "led", "shaped", "delivered", "enabled", and "helped teams operate" where accurate.

Maintain the same current examples unless better public-safe examples are provided:

- Serverless Data Pipeline - Public Sector
- PSA Platform - Professional Services Firm
- Secure Landing Zone - Formula E Trackside Analytics
- Regulated Data Centre Exit - Major UK Bank
- AI Chat Assistant - UK Water Company

Copy should be outcome-led rather than case-study heavy.

### 5. Pinned Repo Strategy

Use GitHub pinned repositories to support the profile story, but do not add a forward-looking reference-project claim to the README.

Recommended future pinned repo set:

- Wiz + Terraform repo: security posture, infrastructure as code, cloud governance.
- Secure Kubernetes demo: platform engineering and secure-by-default cluster patterns.
- AI assistant / Gemini demo: practical AI enablement for useful internal tools.
- Serverless data pipeline demo: GCP/serverless delivery and data governance.
- Platform landing zone template: repeatable foundations and architecture leadership.
- Developer productivity / AI dev tooling repo: how teams build, not just what they deploy.

Do not claim these repos already exist unless they are present and public.

### 6. Tools And Credentials

Move badges and certifications toward the bottom so they support the story instead of dominating it. Include:

- Google Cloud certifications
- Wiz accreditation/training
- Google Cloud, Kubernetes, Terraform, Cloud Run, Firebase, BigQuery
- Gemini, AI tooling, DevSecOps, architecture

### 7. Sectors

Keep sectors, but make them quieter. They are credibility signals, not the main story.

## Visual Direction

GitHub README rendering is limited, so the design should rely on hierarchy, spacing, and concise copy rather than heavy HTML styling.

Use:

- Centred top section.
- Short horizontal rules to separate major regions.
- A three-column table for capability blocks.
- Minimal, grouped badges.
- No GitHub stats, streak widgets, trophy widgets, or large animated elements.
- No broken banner reference unless a real `banner.png` is committed.

The final README should feel tidy, senior, and easy to scan on both desktop and mobile GitHub.

## Implementation Notes

- Modify `README.md` only unless a real asset is added.
- Keep Markdown and HTML GitHub-compatible.
- Use ASCII punctuation in prose where practical.
- Do not add claims about public repos that are not available yet.
- Keep the page readable even if shields.io badges fail to load.

## Acceptance Criteria

- The top of the README clearly positions Caz for broad technical leadership.
- AI is present as a practical enablement thread, not hype or the main brand.
- The body is less badge-heavy than the current README.
- Selected work reads as proof of senior delivery and leadership.
- Future pinned repo suggestions remain implementation guidance and are not presented as public work in the README.
- The README remains valid GitHub-flavoured Markdown.
