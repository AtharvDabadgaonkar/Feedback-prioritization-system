# Signalboard — User Feedback & Feature Prioritization System

- Turn 1,000+ scattered signals into one ranked roadmap.

Signalboard is an interactive product case study (SaaS) that shows how raw, messy
user feedback becomes a clear, defensible product roadmap. Feedback arrives
everywhere — surveys, support tickets, and reviews — so this workspace pulls it
all into one place, scores every idea with RICE, and outputs a prioritized
roadmap you can defend to any stakeholder.

It ships as a single self-contained HTML file — no build step, no dependencies,
no package manager. Just open it in a browser and it runs.

## Live demo

Once GitHub Pages is enabled, the demo is live at:
https://AtharvDabadgaonkar.github.io/Feedback-prioritization-system/

## What it does

Signalboard walks through the full prioritization loop a product manager runs
every quarter:

1. Aggregate — collect feedback from three separate channels into one stream.
2. Cluster — group 1,000+ raw inputs into a handful of clear themes
   (conceptually done with SQL and Python).
3. Score — rate each theme on RICE so loud-but-low-impact requests can't jump
   the queue.
4. Rank and tier — sort everything into a Now / Next / Later roadmap, with the
   option to manually override.

The feedback comes from three sources: surveys (NPS and in-app), support tickets
(Zendesk import), and product reviews (app stores and G2). All three feed a
single pool of 1,000+ inputs, clustered into 6 themes.

## Key features

- A live count-up dashboard showing inputs streaming in from each source.
- RICE scoring applied to every theme, with the score shown on each row.
- A drag-to-reorder roadmap — drag any row to override the ranking and watch the
  Now / Next / Later tiers recompute instantly.
- Sort modes to switch between RICE score, Reach, or your own manual order.
- A North Star metric and OKRs framing, so every feature ties back to a goal.
- A responsive, animated UI with a reduced-motion fallback for accessibility.

## The scoring model: why RICE, not gut feel

Every theme gets four honest inputs instead of opinions. RICE stands for:

- Reach — how many users this touches per quarter.
- Impact — how much it moves the metric, per user.
- Confidence — how much evidence backs the estimate.
- Effort — person-weeks to build and ship it.

The formula is:

RICE = (Reach × Impact × Confidence) ÷ Effort

A higher score means a higher spot in the roadmap.

## Tech stack

The front end is plain HTML, CSS, and vanilla JavaScript, all inline in one file.
Fonts (Space Grotesk, Inter, JetBrains Mono) load from Google Fonts, which is the
only external resource. The analysis side is conceptually done with SQL and
Python for clustering and theme aggregation, and the methodology uses RICE
prioritization, a North Star metric, and OKRs.

## Run locally

Just open index.html in any modern browser. No install, no server, no build.

## Project structure

- index.html — the entire demo, all HTML, CSS, and JS inline.
- README.md — this file.
- HANDOFF.md — internal context notes.

## Author
Atharv Dabadgaonkar
