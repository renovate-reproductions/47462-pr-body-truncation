# Truncated vulnerability PR body

Reproduction for [renovatebot/renovate#47462](https://github.com/renovatebot/renovate/pull/47462), from [discussion #47461](https://github.com/renovatebot/renovate/discussions/47461).

`jackson-databind` `2.9.0` is affected by so many OSV advisories that the advisory section alone exceeds the PR body limit.
`osvVulnerabilityAlerts` raises a vulnerability PR for it, with automerge enabled.

## Current behavior

The PR body is cut inside the advisories.
The `### Configuration` section (with `**Automerge**: Enabled.`), the rebase checkbox and the `renovate-debug` comment are missing.

## Expected behavior

The advisories are cut instead.
The `### Configuration` section, the rebase checkbox and the `renovate-debug` comment are kept at the end of the PR body.
