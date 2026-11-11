# PM_Docs
Product Manager Docs regarding zero until the first users

## Claude Code harness

This repo enables the [ECC](https://github.com/affaan-m/ECC) plugin (`ecc@ecc`, pinned to `v2.2.3`) at project scope via `.claude/settings.json`, so every Claude Code session here, local or cloud, picks it up automatically. ECC's `common` rule pack lives in `.claude/rules/ecc/common` (plugins can't ship rules).

To upgrade, bump `ref` in `.claude/settings.json` and re-copy `rules/common` from the matching ECC tag.

## Social media research skills

The 13 [ScrapeCreators social-media-research-skills](https://github.com/ScrapeCreators/social-media-research-skills) (MIT) are vendored into `.claude/skills/` at upstream commit `64ba7b4`. They need a ScrapeCreators API key: store it as a network secret for `api.scrapecreators.com` (header `x-api-key`) on the cloud environment, or export `SCRAPECREATORS_API_KEY` locally. Never commit the key.

To upgrade, re-copy `skills/` from the upstream repo and update the commit above.
