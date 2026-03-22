---
name: Professionalize GitHub Profile README
description: "Rewrite a GitHub profile README into a high-technical, senior-grade professional profile"
argument-hint: "Paste current README content or describe the profile style you want"
agent: agent
---
Create or refine a GitHub profile `README.md` for the profile repository (username repository).

Requirements:
- Keep tone technical, credible, and concise.
- Use accurate project information only; do not invent metrics or achievements.
- Prioritize architecture depth over generic portfolio language.
- Keep markdown readable on both mobile and desktop.
- Prefer clean formatting over decorative clutter.
- Write like a hiring manager or senior engineer is scanning for technical ownership.

Inputs to use:
- Selected text or current `README.md` content.
- Public repositories and pinned projects if available.
- Any user-provided career focus (internships, open source, specific domain).

Output format:
1. Return the full improved `README.md` content.
2. Then provide a short "Why this works" section with 3-5 bullets.
3. Then provide 2 optional variants: `Minimal` and `Recruiter + Technical` (short outlines only).

Quality bar:
- No hype wording, no filler, no fake metrics.
- Each major project should include stack + architecture + implementation detail.
- Highlight concrete engineering signals: contracts, performance constraints, runtime behavior, tooling, and deployment path.
- Language and grammar should be polished.
