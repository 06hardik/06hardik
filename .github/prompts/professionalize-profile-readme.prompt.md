---
name: Professionalize GitHub Profile README
description: "Rewrite or improve a GitHub profile README to look professional, concise, and recruiter-friendly"
argument-hint: "Paste current README content or describe the profile style you want"
agent: agent
---
Create or refine a GitHub profile `README.md` for the profile repository (username repository).

Requirements:
- Keep tone professional, confident, and concise.
- Use accurate project information only; do not invent achievements.
- Include these sections when possible: About, Featured Projects, Tech Stack, Current Focus, Contact.
- Keep markdown readable on both mobile and desktop.
- Prefer clean formatting over visual clutter.

Inputs to use:
- Selected text or current `README.md` content.
- Public repositories and pinned projects if available.
- Any user-provided career focus (internships, open source, specific domain).

Output format:
1. Return the full improved `README.md` content.
2. Then provide a short "Why this works" section with 3-5 bullets.
3. Then provide 2 optional variants: `Minimal` and `Technical` (short outlines only).

Quality bar:
- No hype wording, no filler, no fake metrics.
- Clear project descriptions in one line each.
- Language and grammar should be polished.
