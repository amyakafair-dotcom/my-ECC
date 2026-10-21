# my-ECC

This repo turns on [ECC (Everything Claude Code)](https://github.com/affaan-m/ECC) whenever it's opened in Claude Code.

- `.claude/settings.json` adds the ECC plugin marketplace and turns on the `ecc@ecc` plugin (its agents, skills, commands and hooks).
- `.claude/rules/ecc/` holds ECC's rule packs. The `common` rules always load. Each language rule loads only for matching files.
- `.claude/agents/` holds all ECC agents (copied from ECC commit `90606c8`, MIT license in `LICENSE-ECC`). They load in any session that has this repo.
- `.claude/agents/` also holds the agents from [The Agency](https://github.com/msitarzewski/agency-agents) (commit `4e3ac3c`, MIT license in `LICENSE-agency-agents`), installed with its `scripts/install.sh --tool claude-code`.
- `.claude/skills/hairline-create/` is the skill from [hairline](https://github.com/lucasmarkes/hairline) (commit `37d2e78`, MIT license in that folder). It draws new Hairline figures.

To get updated rules, copy `rules/` again from the ECC repo.
