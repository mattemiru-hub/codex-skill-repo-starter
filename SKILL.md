---
name: codex-skill-repo-starter
description: Build and polish public-ready Codex skill repositories with the right structure, clarification rules, documentation, scripts, and QA guardrails. Use when the user wants to create a new Codex skill repo, split bootstrap logic into a separate repo, or package a skill repo so another user can install and use it cleanly.
---

# Codex Skill Repo Starter

## Quick Start

- Inspect the user request and source artifacts first.
- Read `references/clarification-rules-vi.md` before mapping important fields or making structural changes.
- Read `references/domain-contract-vi.md` before building the main output.
- Read `references/qa-checklist-vi.md` before final delivery.
- Read `references/prompt-template-vi.md` only when the user asks for a reusable prompt.

## Workflow

1. Inspect the input files, current state, schema, and expected deliverable.
2. Run the clarification gate before mapping any critical fields or changing structure.
3. Map inputs to business roles instead of assuming fixed names.
4. Execute the repo-building workflow defined in `references/domain-contract-vi.md`.
5. Validate the output using `references/qa-checklist-vi.md`.
6. Save a stable final result and summarize any compromises clearly.

## Clarification Gate

Before doing the main build, decide whether the task can be executed with high confidence.

Ask the user before proceeding if any of these are unclear:

- the main source file or sheet
- the key repo purpose, audience, or install flow
- the expected final deliverable format
- whether to preserve an existing output or rebuild from scratch
- whether a required script, reference, or example should live in the repo

Do not guess low-confidence business-critical mappings.
If confidence is below high confidence, stop and ask.

## Required Question Style

Ask only the minimum short concrete questions required to continue.

Preferred style:

1. Nguồn dữ liệu chính là file hoặc sheet nào?
2. Repo này dùng để làm đúng việc gì?
3. Bạn muốn polish repo hiện tại hay dựng repo mới từ đầu?

Do not ask broad open-ended questions when a short targeted question will unblock the work.

## Non-Negotiables

- Preserve the approved user-facing experience, not a rough draft.
- Do not mix bootstrap tooling into an unrelated domain repo when it should live separately.
- Keep colors, labels, wording, and logic stable and meaningful.
- Validate the output before final delivery.

## Deliverables

- Final working artifact
- Short summary of what was built
- Short clarification summary when important mappings were confirmed by the user
- List of any unresolved limitations
