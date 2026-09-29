# Vendored skills

Third-party Agent Skills, copied here unmodified. They are **not** part of the Design Lore
family: no `lore/*.jsonl`, not in `INDEX.tsv`, not registered in `repackage-skills.py`.
`install.sh` symlinks them into `~/.claude/skills/` alongside the Design Lore skills.

To update one, re-copy it from upstream rather than editing in place.

| Skill | Upstream | Path in upstream | Commit vendored |
|---|---|---|---|
| `shopify-liquid-themes` | [benjaminsehl/liquid-skills](https://github.com/benjaminsehl/liquid-skills) | `skills/shopify-liquid-themes` | `483f969` |
| `liquid-theme-standards` | [benjaminsehl/liquid-skills](https://github.com/benjaminsehl/liquid-skills) | `skills/liquid-theme-standards` | `483f969` |
| `liquid-theme-a11y` | [benjaminsehl/liquid-skills](https://github.com/benjaminsehl/liquid-skills) | `skills/liquid-theme-a11y` | `483f969` |
| `cro` | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | `skills/cro` | `5b2c000` |
| `marketing-psychology` | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | `skills/marketing-psychology` | `5b2c000` |
| `web-design-guidelines` | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) | `skills/web-design-guidelines` | `063bee9` |
| `frontend-design` | [anthropics/skills](https://github.com/anthropics/skills) | `skills/frontend-design` | `8a1541c` |

## Notes

- `cro` and `marketing-psychology`: upstream `evals/` folders were not vendored.
- `frontend-design`: ships its own `LICENSE.txt` (Anthropic); terms there apply.
- `web-design-guidelines`: a thin wrapper — it fetches its actual rules at runtime from
  `raw.githubusercontent.com/vercel-labs/web-interface-guidelines/main/command.md`.
- `cro` and `marketing-psychology` read `.agents/product-marketing.md` from the working
  project if present.

Vendored 2026-09-29.
