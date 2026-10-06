# Changelog

## [0.15.0](https://github.com/ther3ptil31987-prog/frugal/compare/v0.14.1...v0.15.0) (2026-10-06)


### Features

* /frugal:models command for per-project model overrides ([0727178](https://github.com/ther3ptil31987-prog/frugal/commit/07271787364dce275a22fbd112bffca03951ca00))
* block reasoning-tier agents at spawn via guard_expensive ([876e8f4](https://github.com/ther3ptil31987-prog/frugal/commit/876e8f4cda13f9bb4329d0536541449e117d5034))
* context-handoff rule - pass pointers, not pasted content ([3f9e0a9](https://github.com/ther3ptil31987-prog/frugal/commit/3f9e0a9360a93bb35c5c8babdf549dbd2e26978b))
* core routing skill with decision table and escalation protocol ([3a4c51c](https://github.com/ther3ptil31987-prog/frugal/commit/3a4c51c8ea28022205e3b993a5bc562c19f8be5b))
* cost report script and router-stats skill ([0ad3ac5](https://github.com/ther3ptil31987-prog/frugal/commit/0ad3ac5b939a3cacfab8c0cafd45797570873eda))
* enforce routing via SessionStart and UserPromptSubmit hooks ([8586d18](https://github.com/ther3ptil31987-prog/frugal/commit/8586d1819e47388dfcc9a98e5b283ea2aec7557c))
* five tiered worker agents with footer contract ([7abc1d2](https://github.com/ther3ptil31987-prog/frugal/commit/7abc1d205e7f091127825b2f250f012d31c0ee4e))
* format the router report as a bill ([#20](https://github.com/ther3ptil31987-prog/frugal/issues/20)) ([a0bc930](https://github.com/ther3ptil31987-prog/frugal/commit/a0bc9308cdce94950ae5563593cd7c19264249b7))
* gate sensitive data before tier selection ([#18](https://github.com/ther3ptil31987-prog/frugal/issues/18)) ([1982c6c](https://github.com/ther3ptil31987-prog/frugal/commit/1982c6ca09c12184a42009b583f9a94c5e45c297)), closes [#17](https://github.com/ther3ptil31987-prog/frugal/issues/17)
* honest net-cost savings and per-run duration ([90dedf6](https://github.com/ther3ptil31987-prog/frugal/commit/90dedf6bb59ba9ac14c05c23fde8be37bb701a5d))
* inline-exploration budget guard and bright-line delegation rule ([e2e8381](https://github.com/ther3ptil31987-prog/frugal/commit/e2e83816e6983091489cabe75bf308b5c7f69b21))
* meter session spend and publish a delegation floor ([#30](https://github.com/ther3ptil31987-prog/frugal/issues/30)) ([747da44](https://github.com/ther3ptil31987-prog/frugal/commit/747da449aa25e3a60db6a1e87ea471dc7c4d8bf3))
* metrics-to-routing feedback via SessionStart advice ([c29929e](https://github.com/ther3ptil31987-prog/frugal/commit/c29929e35267d1ecb6d6ea47fade2fcbf9618585))
* on-demand routing eval scenarios and runner ([6d86789](https://github.com/ther3ptil31987-prog/frugal/commit/6d86789236c1a753f727ae425853bbab73635e22))
* optional PreToolUse guard blocking expensive-tier spawns ([8aa9048](https://github.com/ther3ptil31987-prog/frugal/commit/8aa90484464f528992b21194a0fe7359b193cbfa))
* per-session savings table in stats.py ([#5](https://github.com/ther3ptil31987-prog/frugal/issues/5)) ([054f70a](https://github.com/ther3ptil31987-prog/frugal/commit/054f70a540c64476bb030393dd0c9bae4b27a40f))
* plugin scaffold with manifest and marketplace ([5423d6d](https://github.com/ther3ptil31987-prog/frugal/commit/5423d6d332c5f86bee7481fa712391f0f80c0f7b))
* reply caps on mechanic, builder, and sage ([4a4e06d](https://github.com/ther3ptil31987-prog/frugal/commit/4a4e06ddcf97945bcd22e7397ca77ccb31f3ea24))
* savings baseline follows the session's main-loop model ([0cb5f3f](https://github.com/ther3ptil31987-prog/frugal/commit/0cb5f3f187484ff3207058c3e48964e890d16282))
* setup-statusline skill wiring the savings badge on consent ([e6e6974](https://github.com/ther3ptil31987-prog/frugal/commit/e6e69740dedf493e7f5b6c9984a5170a61bd55be))
* statusline savings segment; drop synthetic evals for usage metrics ([981d2c0](https://github.com/ther3ptil31987-prog/frugal/commit/981d2c0ff6766b49aa73638c28b741b432a58cce))
* SubagentStop metrics hook logging tokens and escalations ([2accfdd](https://github.com/ther3ptil31987-prog/frugal/commit/2accfddb377d992625e4ec76a5be12f2417ca8e8))
* token-lean worker output; skip typeless subagent stops in metrics ([15be420](https://github.com/ther3ptil31987-prog/frugal/commit/15be420b50234d1c3c455c0e73c5296352729948))


### Bug Fixes

* eval runner missing --verbose required by stream-json print mode ([cee531f](https://github.com/ther3ptil31987-prog/frugal/commit/cee531fdc6769c3a8c438c206ba13eaa99b503c5))
* eval scenarios run against real fixtures on a sonnet main loop ([f7ad6d1](https://github.com/ther3ptil31987-prog/frugal/commit/f7ad6d13e55b2eff4c8967e0f8061e4aa86199da))
* guard_inline matches search commands after shell prefixes ([911d1c5](https://github.com/ther3ptil31987-prog/frugal/commit/911d1c5b3cdfcd2f9623f678d5f7a31d1af3079d))
* guard_inline no longer counts write-redirected commands ([2c60303](https://github.com/ther3ptil31987-prog/frugal/commit/2c603033d3f6dbec7dcb4fc66b0be90d8f624256))
* metrics measured the main session instead of the subagent ([8a17bd6](https://github.com/ther3ptil31987-prog/frugal/commit/8a17bd61ea8f4188cf1762c314045c87243f90b0))
* only reset inline-search budget on foreground agent dispatch ([#6](https://github.com/ther3ptil31987-prog/frugal/issues/6)) ([09a0f54](https://github.com/ther3ptil31987-prog/frugal/commit/09a0f54ab41bb63fae532a62032c725aab57f1e1))
* read agent transcripts as UTF-8 in log_metrics ([#25](https://github.com/ther3ptil31987-prog/frugal/issues/25)) ([b135a6a](https://github.com/ther3ptil31987-prog/frugal/commit/b135a6aa8f90c5fe523fdf46b0937715f1907ff3)), closes [#22](https://github.com/ther3ptil31987-prog/frugal/issues/22)
* **stats:** current model prices and per-model report rows ([#42](https://github.com/ther3ptil31987-prog/frugal/issues/42)) ([abb568a](https://github.com/ther3ptil31987-prog/frugal/commit/abb568a84feae49c6bd5987cb746e48a50429017))
* stop guard_expensive denying every spawn where python3 is absent ([#26](https://github.com/ther3ptil31987-prog/frugal/issues/26)) ([9272ecc](https://github.com/ther3ptil31987-prog/frugal/commit/9272ecca8356f52cec927292572cf5f0dd2d519f)), closes [#23](https://github.com/ther3ptil31987-prog/frugal/issues/23)
* stop guard_inline counting pipe filters as inline searches ([#29](https://github.com/ther3ptil31987-prog/frugal/issues/29)) ([b27db35](https://github.com/ther3ptil31987-prog/frugal/commit/b27db355871712a91074ffb3bf4cfabf9917ea20))

## [0.14.1](https://github.com/ThomasLangbroek/frugal/compare/v0.14.0...v0.14.1) (2026-10-06)


### Bug Fixes

* **stats:** current model prices and per-model report rows ([#42](https://github.com/ThomasLangbroek/frugal/issues/42)) ([abb568a](https://github.com/ThomasLangbroek/frugal/commit/abb568a84feae49c6bd5987cb746e48a50429017))

## [0.14.0](https://github.com/ThomasLangbroek/frugal/compare/v0.13.3...v0.14.0) (2026-07-27)


### Features

* meter session spend and publish a delegation floor ([#30](https://github.com/ThomasLangbroek/frugal/issues/30)) ([747da44](https://github.com/ThomasLangbroek/frugal/commit/747da449aa25e3a60db6a1e87ea471dc7c4d8bf3))

## [0.13.3](https://github.com/ThomasLangbroek/frugal/compare/v0.13.2...v0.13.3) (2026-07-27)


### Bug Fixes

* stop guard_inline counting pipe filters as inline searches ([#29](https://github.com/ThomasLangbroek/frugal/issues/29)) ([b27db35](https://github.com/ThomasLangbroek/frugal/commit/b27db355871712a91074ffb3bf4cfabf9917ea20))

## [0.13.2](https://github.com/ThomasLangbroek/frugal/compare/v0.13.1...v0.13.2) (2026-07-27)


### Bug Fixes

* stop guard_expensive denying every spawn where python3 is absent ([#26](https://github.com/ThomasLangbroek/frugal/issues/26)) ([9272ecc](https://github.com/ThomasLangbroek/frugal/commit/9272ecca8356f52cec927292572cf5f0dd2d519f)), closes [#23](https://github.com/ThomasLangbroek/frugal/issues/23)

## [0.13.1](https://github.com/ThomasLangbroek/frugal/compare/v0.13.0...v0.13.1) (2026-07-27)


### Bug Fixes

* read agent transcripts as UTF-8 in log_metrics ([#25](https://github.com/ThomasLangbroek/frugal/issues/25)) ([b135a6a](https://github.com/ThomasLangbroek/frugal/commit/b135a6aa8f90c5fe523fdf46b0937715f1907ff3)), closes [#22](https://github.com/ThomasLangbroek/frugal/issues/22)

## [0.13.0](https://github.com/ThomasLangbroek/frugal/compare/v0.12.0...v0.13.0) (2026-07-22)


### Features

* format the router report as a bill ([#20](https://github.com/ThomasLangbroek/frugal/issues/20)) ([a0bc930](https://github.com/ThomasLangbroek/frugal/commit/a0bc9308cdce94950ae5563593cd7c19264249b7))

## [0.12.0](https://github.com/ThomasLangbroek/frugal/compare/v0.11.1...v0.12.0) (2026-07-22)


### Features

* gate sensitive data before tier selection ([#18](https://github.com/ThomasLangbroek/frugal/issues/18)) ([1982c6c](https://github.com/ThomasLangbroek/frugal/commit/1982c6ca09c12184a42009b583f9a94c5e45c297)), closes [#17](https://github.com/ThomasLangbroek/frugal/issues/17)

## 0.11.1 - 20-07-2026
- guard_inline resets the inline-search budget only on foreground (blocking) agent dispatches; background dispatches (the default) keep the counter climbing, so inline discovery racing a background worker is still throttled instead of getting a fresh budget.

## 0.10.0 - 13-07-2026
- Per-session savings table in the stats report: one row per `session_id`, newest first, using the same net-vs-baseline definition as the totals so rows reconcile. Sessions that ran opus-on-opus show negative savings (the true delta, no cheaper tier to route to).

## 0.9.0 - 10-07-2026
- Honest savings: net cost includes the worker reply re-ingested at main-loop rates (`handoff_output_tokens`, final response only); statusline and report both use it.
- Per-run `duration_ms` from transcript timestamps; average duration per agent in the report.
- Metrics-to-routing feedback: `stats.py --advice` flags miscalibrated routes (escalation >30%, net >= baseline, fat handoffs) at SessionStart; silent when healthy.
- Reply caps on mechanic (150 words), builder (250), sage (500, overflow to scratch file); code never echoed back.
- Context-handoff routing rule: pass pointers, not pasted content.
- guard_inline fixes: write-redirected commands (`cat >> f`) no longer counted; shell prefixes (`cd x && grep`) no longer dodge the counter.

## 0.8.0 - 09-07-2026
- Savings baseline follows the session's main-loop model instead of always the top tier.

## 0.7.2 - 09-07-2026
- Dependency bumps (GitHub Actions checkout, setup-python).

## 0.7.1 - 09-07-2026
- Pricing verification date refresh; first change through the gated PR flow.

## 0.7.0 - 08-07-2026
- `/frugal:models`: per-project model overrides via `.claude/routing-overrides.md`.

## 0.6.0 - 08-07-2026
- Token-lean worker output: scout/extractor compress replies, builder ships the shortest working diff.
- Metrics ignore typeless subagent stops (internal machinery, not routed work).

## 0.5.1 - 08-07-2026
- Metrics measured the main session instead of the subagent; usage snapshots double-counted; escalation false positives from the policy text. All fixed; old metrics invalidated.

## 0.5.0 - 08-07-2026
- Inline-exploration budget guard (PreToolUse): denies search-type calls past `FRUGAL_INLINE_BUDGET` per prompt, pointing at the cheap workers.
- Bright-line rule in the routing policy: third search/list/read operation on one question means delegate.

## 0.4.0 - 08-07-2026
- Enforcement hooks: SessionStart injects the routing policy, UserPromptSubmit re-pins it each prompt. Routing no longer depends on manually invoking the skill.

## 0.3.0 and earlier - 07-2026
- Routing skill and decision table, five worker agents, escalation protocol.
- Metrics hook, cost report (`/frugal:router-stats`), statusline savings segment, optional expensive-tier guard.
