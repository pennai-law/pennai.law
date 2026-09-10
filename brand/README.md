# Brand pipeline — internal identity only (from 2026-09-10)

> These scripts generate the W2 lockup (tech shield + Rajdhani wordmark), which left the public site on 2026-09-10 because it modifies the Penn shield and constitutes a unit-built identity system, both barred by `law.upenn.edu/brand`. The site now uses the official Penn Carey Law logo, unmodified (`static/pcl-logo-reverse.png`, from the Communications logo package PEN-23969). The W2 mark remains in use for internal identity only, the Slack icon and the GitHub org avatar (Polk's decision), so these scripts stay runnable for that purpose. Never put their output on a public web surface. Decision: Box `Lab/design/2026-09-10-brand-compliance.md`.


Generates the Penn Carey Law AI Project lockup (W2: PENN CAREY LAW · PENNAI.LAW eyebrow line,
text block fitted to the shield's ink mass). Spec: docs/superpowers/specs/2026-07-29-site-redesign-design.md §7.

- `build_brand.py` — base pipeline: HarfBuzz shaping + fontTools outlining. Historical: emits the
  pre-URL mark. Kept because build_w2.py execs its helper functions.
- `build_w2.py` — the production mark. Emits lockup-color.svg / lockup-white.svg to
  ~/Downloads/PennCareyLawAIProject-brand-2026-07/; copy into static/ as heading-color.svg /
  heading-white.svg.

Requirements: `pip install uharfbuzz fonttools`, plus `~/Library/Fonts/Rajdhani-Bold.ttf`.
Note: build_w2.py execs the helper block of build_brand.py from its own directory — keep them together.
This directory is not published (Hugo publishes only content/, static/, assets/).
