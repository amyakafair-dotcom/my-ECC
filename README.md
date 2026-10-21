# my-ECC

This repo turns on [ECC (Everything Claude Code)](https://github.com/affaan-m/ECC) whenever it's opened in Claude Code.

- `.claude/settings.json` adds the ECC plugin marketplace and turns on the `ecc@ecc` plugin (its agents, skills, commands and hooks).
- `.claude/rules/ecc/` holds ECC's rule packs. The `common` rules always load. Each language rule loads only for matching files.
- `.claude/agents/` holds all ECC agents (copied from ECC commit `90606c8`, MIT license in that folder). They load in any session that has this repo.

To get updated rules, copy `rules/` again from the ECC repo.
