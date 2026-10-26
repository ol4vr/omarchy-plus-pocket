# Omarchy+ ownership

This repository is the independently controlled Omarchy+ source for Pocket.
It preserves the complete upstream history and the exact runtime accepted on
Hugin without changing Pocket's behavior.

## Provenance

- Upstream repository: <https://github.com/jrmmhm/omarchy-pocket>
- Audited upstream commit: `81c90494f812c9f58a66e8a0e68a78c59197c1c0`
- Audited version: `0.5.0`
- Upstream license: MIT; the original `LICENSE` and attribution are unchanged.
- Omarchy+ security decision: GO for the exact audited runtime only.

The accepted runtime files `BarWidget.qml`, `Model.js`, and `manifest.json`
are byte-identical to the audited upstream commit. The plugin ID remains
`jrmmhm.pocket` so existing Pocket membership, pin, lock, and bar-placement
settings continue to apply.

## Ownership and updates

`origin` is the Omarchy+-owned repository. The original repository is retained
as fetch-only `upstream`; it is never a deployment or automatic-update
authority. Omarchy+ BASE installs an exact owned commit and does not need the
upstream repository at recovery time.

Every future upstream revision requires a new complete third-party security
review, compatibility validation, and owner acceptance before it can be
selected. Do not merge or fast-forward upstream automatically.

Run the existing upstream validation with:

```text
tests/run.sh
```

The central Omarchy+ repository owns Hugin placement, initial clean-home
membership, preserved-home state, reconciliation, and rollback policy.
