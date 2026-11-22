# RESEARCH.md — news-image-20261121 V2 "The Second Overtime"

One-page newspaper summing up world news on **Saturday 21 November 2026**:
36 stories (3 leads, 11 features, 22 briefs) across 7 regions, a numbered
world map, 6 key numbers, and a DATE CHECK box listing 6 big 19–20 Nov
stories deliberately excluded.

## Method

- Facts re-verified from primary sources dated 21 Nov 2026 (see the full
  source table in the build notes: 3 leads + 11 features + 22 briefs, each
  with source + date). Two stories V1 could only list as scheduled
  (BepiColombo Mercury orbit insertion, Cargo Dragon splashdown) are now
  confirmed from ESA/NASA/SpaceX reporting dated 21 Nov 2026 and promoted
  to features. The COP31 final text circulated in the early hours of
  Sunday 22 Nov — NOT 21 Nov — so the image only says the talks worked
  through Saturday in a second overtime day.
- Region counts (by story location): Europe 13, Americas 10, Asia-Pacific 3,
  Africa 3, Middle East 2, Oceania 2, World/Space 3 = 36.
- All 36 stories happened, or were first reported, on 21 Nov 2026 in at
  least one time zone. Claims are attributed, not stated as fact (e.g. the
  Anthropic maths claim is labelled unproven).

## Production

- `render.html` — static page, local fonts, inline SVG scenes drawn fresh
  in this session, no network, no JavaScript. Rendered with headless
  Chromium to `entry.png` (1024×1024, PNG).
- Fonts: Gelasio + Source Sans 3 (SIL Open Font License 1.1), woff2 latin,
  downloaded fresh from Google Fonts.
- `main.py` (stdlib only) copies `entry.png` to `$MAKEFUN_OUTPUT_DIR/entry.png`.
- All drawings are original vector scenes; no photos, no model-generated
  images, no clip-art. No real person is depicted recognisably.

## Verification (build session, 22 Nov 2026)

- `main.py` run twice: byte-identical output (sha256 recorded in build notes).
- `entry.png`: 1024×1024, PNG, under 1 MiB.
- Render: 0 console errors, 0 failed requests.
- Contrast measured (WCAG): lowest pair 7.75:1 (red on paper); all text
  pairs ≥ 4.5:1, all small text ≥ 7:1.
- Smallest body text 10 px on the 1024 canvas; art-embedded data labels
  ≥ 10 px effective after measurement (lead strips 9.8 px, map pins 8.5 px — see gates).
- Viewed at 1024, 512, 390 and 300 px wide; masthead, KPI numbers and hero
  headline legible at 390 px; every letter read at 100% zoom.
