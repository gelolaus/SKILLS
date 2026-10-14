# SKILLS

A collection of agent skills by [Angelo Laus](https://gelolaus.com). Each skill lives in its own folder under `skills/` and works with Claude Code and other agents that read `SKILL.md`.

## Skills

| Skill | What it does |
| ----- | ------------ |
| [conventional-commits](skills/conventional-commits/SKILL.md) | Writes commit messages in Angelo's Conventional Commits style: `type(scope): lowercase imperative subject` with a terse bullet body. Outputs the message only and never runs `git commit`. |

## Install

Install a skill with the skills CLI:

```bash
npx skills add gelolaus/SKILLS@conventional-commits
```

Add `-g` to install it for all your projects instead of only the current one.

### Manual install

Clone the repo and copy the skill folder you want into your skills directory (`~/.claude/skills/` for Claude Code, or `.claude/skills/` inside a single project):

```bash
git clone https://github.com/gelolaus/SKILLS
cp -r SKILLS/skills/conventional-commits ~/.claude/skills/
```

On Windows PowerShell:

```powershell
Copy-Item -Recurse SKILLS\skills\conventional-commits $HOME\.claude\skills\
```

## Adding a skill

Create `skills/<skill-name>/SKILL.md` with `name` and `description` frontmatter, then add a row to the table above.

## License

[MIT](LICENSE)
