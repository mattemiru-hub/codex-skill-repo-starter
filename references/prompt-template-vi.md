# Prompt Template Tiếng Việt

```text
Use $codex-skill-repo-starter to help me with creating public-ready Codex skill repositories with the right structure, clarification rules, documentation, and QA guardrails.

Before doing the main work:
- inspect the source first
- ask short clarification questions if repo boundary, install flow, or deliverables are ambiguous
- do not guess whether this should stay inside an existing domain repo or move to a separate starter repo

Deliverables:
- final repo structure and files
- short summary of what changed
- note any unresolved limitations
```

## Bien the prompt nen dung

```text
Use $codex-skill-repo-starter to turn my current local folder into a public-ready Codex skill repo.

Requirements:
- inspect the current repo first
- decide whether this is a domain repo or a bootstrap repo
- if the boundary is mixed, separate it cleanly
- create or revise SKILL.md, README.md, README_vi.md, agents/openai.yaml, references, scripts, and changelog as needed
- ask me only the minimum questions needed when repo purpose, audience, or install flow is unclear

Deliverables:
- final repo files ready for GitHub
- short explanation of the repo boundary
- short usage note for how another Codex session should use this repo
```
