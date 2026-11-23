# makefun-sitegen-speed-20261122

Faster drop-in for make.fun's makefun-site 1.0.0 static site generator, built for the [site-generator-speed-01-run-20261122 bounty](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) ($100 in USDC, CPU-time race).

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/denz136/makefun-sitegen-speed-20261122/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/denz136/makefun-sitegen-speed-20261122/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

`solve.js` reimplements the hot paths of makefun-site's pipeline (front matter, Markdown, templates, escaping) with byte-identical output, tuned for V8: branchless HTML escaping, char-code lexing, slice-based front-matter parsing and allocation-free template loops. ~35% less CPU than the house baseline on the practice set.

## Run

```
node main.ts
```

Reads `/input/cases.json`, writes `/output/answers.json` (override with `MAKEFUN_INPUT_DIR` / `MAKEFUN_OUTPUT_DIR`).

## License

MIT
