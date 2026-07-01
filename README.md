# Codex Skill Repo Starter

GitHub-ready starter repo for creating public-ready Codex skill repositories with the right structure, clarification rules, documentation, and QA guardrails.

## What this repo gives you

- a reusable `SKILL.md` entrypoint for a repo-building skill
- clarification-first behavior to reduce low-confidence guessing
- references for repo structure, handoff quality, and ask-before-guess rules
- sample starter content that can be replaced quickly
- install and bootstrap scripts

## Quick start

1. Copy this repo into your local Codex skills folder with `scripts/install_local_skill.ps1`.
2. Call `$codex-skill-repo-starter` in Codex when you want a new skill repo.
3. Ask it to scaffold or polish a repo for the domain you want.
4. Use `scripts/init_standard_skill_repo.ps1` when you want a ready-made local scaffold first.

## Folder structure

```text
.
├── SKILL.md
├── README_vi.md
├── agents/
│   └── openai.yaml
├── examples/
│   └── README.md
├── references/
│   ├── clarification-rules-vi.md
│   ├── domain-contract-vi.md
│   ├── prompt-template-vi.md
│   ├── qa-checklist-vi.md
│   └── repo-packaging-playbook-vi.md
├── sample-output/
│   └── README.md
├── scripts/
│   ├── init_standard_skill_repo.ps1
│   └── install_local_skill.ps1
├── CHANGELOG.md
└── LICENSE
```

## Install for Codex

```powershell
powershell -ExecutionPolicy Bypass -File .\scripts\install_local_skill.ps1
```

## Bootstrap a new repo

```powershell
powershell -ExecutionPolicy Bypass -File .\scripts\init_standard_skill_repo.ps1 `
  -TargetPath "C:\path\to\new-skill-repo" `
  -SkillName "my-new-skill" `
  -DisplayName "My New Skill" `
  -DomainSummary "the exact job this skill should own"
```

## Notes

- Use this repo when the job is creating or polishing other skill repos, not when the job is the business domain itself.
- Replace the starter placeholders with real domain rules as soon as the new repo exists.
- Keep the clarification rules strict enough that the AI asks before guessing critical mappings.
