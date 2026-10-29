# PM_Docs
Product Manager Docs regarding zero until the first users

## Claude Code harness

This repo enables the [ECC](https://github.com/affaan-m/ECC) plugin (`ecc@ecc`, pinned to `v2.2.3`) at project scope via `.claude/settings.json`, so every Claude Code session here, local or cloud, picks it up automatically. ECC's `common` rule pack lives in `.claude/rules/ecc/common` (plugins can't ship rules).

To upgrade, bump `ref` in `.claude/settings.json` and re-copy `rules/common` from the matching ECC tag.
