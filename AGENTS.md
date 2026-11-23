# token-radar-01 final entry instructions

- Work only in this repository. Do not modify the official kit, baseline, COMPLIANCE.md, STRATEGY.md, MODEL_SPEC.md, or anything outside `work/final`.
- This is a Node 22 program using only the standard library. No network access at runtime, no environment secrets, no dynamic code execution.
- `main.ts` reads `/input/snapshot.json` in the grader, writes `board.json`, `data.js`, copies `dashboard/` and `screenshots/`, then writes `dossier.json` with `vendor/makefun-board.ts`.
- Keep `vendor/makefun-board.ts` unchanged. Write `main.ts`, `lib/model.ts`, and all dashboard files freshly; do not copy the starter's implementation.
- The board must cover all 40 slugs in `snapshot.watchlist` and add early protocols from the snapshot. Use "records no token" wording, never "has no token".
- Implied value must come only from `tvl_usd`, `change_7d`, `listed_at`, and `as_of`, through one explicit formula. Mark imputed values. Never hardcode protocol names or predict token issuance.
- Farm steps must be concrete, 3-12 strings per row, each 20-600 characters, with action, dollar cost, duration, and risk. Capital tiers and holding windows are assumptions and must be labelled as such.
- The dashboard must be static and offline: index.html plus CSS and JS, sortable and filterable, with a detail view. No http:// or https:// in HTML attributes, CSS files, or JavaScript imports. Visible text may mention sources.
- Keep total dashboard source under 65,536 bytes. Keep output deterministic: no Date.now(), Math.random(), network, or environment lookups in program logic.
- Do not create a GitHub repository, commit, submit, sign, pay, or connect a wallet. Deliver local files only.
