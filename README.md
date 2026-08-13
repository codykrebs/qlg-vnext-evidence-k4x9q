# QLG Intelligence vNext — visual-fidelity evidence

Evidence captures for the QLG Intelligence dashboard redesign (mockups are the
binding visual references; all rendered numbers are live runtime data, never
mockup values). One folder per route as each calibration pass lands.

## billing/ — Billing Settlement Flow (mockup 03) — 2026-08-13 craftsmanship pass

Captured from the deployed Netlify draft preview (commit `d31c892` on
`design/qlg-vnext-relay`), viewport 1536×1024 CSS px, DSF 1, dark,
America/New_York, reduced motion, fonts loaded.

| File | What it is |
|---|---|
| `reference-mockup-03.png` | The binding reference mockup (1536×1024) |
| `before-2026-08-13.png` | Production Billing before this pass |
| `after-desktop-1536x1024.png` | This pass, desktop, live data |
| `after-mobile-390x844.png` | This pass, mobile 390×844 |
| `overlay-50.png` | 50% blend of reference over implementation |
| `region-1-header.png` … `region-6-tabs.png` | Six work-order regions, reference above the teal separator, implementation below |
| `anchor-deltas.json` | Region boundary positions vs reference targets (±12px tolerance; 11/11 pass) |

Region bands at 1536×1024 (reference y-coordinates): header 0–188,
stage/status 188–308, signal cards 316–426, settlement flow 432–660,
working queues 664–938, local tabs 945–1003.

Known data-driven differences from the mockup (live values, honest states):
static canonical cycle chip instead of a period dropdown (no selector exists);
canonical stream stages (Ready / Waiting-on-# / Invoiced; To-enter / Entered)
with dashed ghost segments for tracked-but-$0 stages; per-item magnitude bars
instead of invented history sparklines; coverage in truth-strip slot 4;
Confirm stage and exception owners read "Not tracked"; sends execute in the
audited queue island below the fold.
