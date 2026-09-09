# Agentic Coding 101: Foundation — skills

Devpost Learning Hackathon curriculum, packaged as agent skills. Works in any harness that reads `SKILL.md` (Claude Code, Codex, Cursor, …).

## Install

```
npx skills add devpost/ai-coding-101-skills --all -y
```

Prerequisites: **node** and **git** installed, and an empty folder set aside for your project.

## The sequence

| Skill | What happens | Writes |
|---|---|---|
| `1-start` | Short interview so the agent can pitch everything at your level | `docs/learner-profile.md` |
| `2-plan` | The heart of the course: scope → product → technical plan, reviewed with you at each step | `docs/scope.md`, `docs/prd.md`, `docs/spec.md` |
| `3-build` | Plan becomes ordered build steps; the agent builds, verifies, and commits each one (learn or fast mode) | `docs/checklist.md`, your app |
| `4-ship` | Give your two peer reviews, make the app reachable (live URL or video), draft your Devpost submission | submission text |

Invoke each skill by name in your agent. Starting a fresh conversation between skills is fine — the `docs/` files carry the context forward.

## Layout

```
skills/<name>/SKILL.md          the skill
skills/<name>/templates/        document templates the skill fills in
skills/<name>/references/       deeper material the skill reads on demand
```

## How progress is tracked

There is no progress file. The `docs/` folder is the state:

- Each planning document (`scope.md`, `prd.md`, `spec.md`, `checklist.md`) carries `status: draft | approved` in its frontmatter. Skills save a draft as soon as one exists and flip it to `approved` only when the learner explicitly signs off.
- `learner-profile.md` is about the learner, never about progress. It exists or it doesn't.
- `checklist.md` tracks the build itself through its `- [ ]` / `- [x]` boxes, plus the git log.

Every skill opens by listing `docs/`, reading those status lines, saying back where the learner is, and routing — forward to the right skill if they're behind, or to the first unfinished thing if they're mid-way. So a fresh conversation at any point costs nothing.
