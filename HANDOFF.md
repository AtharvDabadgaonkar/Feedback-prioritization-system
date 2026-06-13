# HANDOFF - User Feedback & Feature Prioritization System

> Context file for any LLM/agent working on this repo. Read this first.

## What this repo is

A single self-contained interactive product case study (SaaS). One HTML file,
no build step, no dependencies, no package manager. It is a prioritization
workspace that aggregates 1,000+ inputs from surveys, support tickets, and
reviews, then ranks features with a live, drag-to-reorder RICE roadmap.

## Layout

- `index.html` - the entire demo. All HTML, CSS, and JS are inline in this one file.
- `README.md` - public-facing project description.
- `HANDOFF.md` - this file (internal agent context, not part of the published page).

## How it runs

Open `index.html` directly in a browser. Hosted on GitHub Pages, it serves at the
repo root automatically because it is named `index.html`. The only external
resource is the Google Fonts stylesheet loaded via `@import`.

## Key interactions

- Rows are drag-to-reorder; dragging a row overrides the ranking and the RICE
  tiers recompute live. Preserve this behavior when editing.

## Ground rules

- Keep everything inline in `index.html`; do not introduce a build step,
  bundler, framework, or external local assets unless explicitly asked.
- This repo is fully self-contained. Do not add links or references to any other
  project or to a shared landing page - earlier those references existed and were
  deliberately removed during the split.
- The numbers in the demo (e.g. 1,000+ inputs) reflect prototype user testing. Do
  not alter them without being asked.
- Do not edit `README.md` or this `HANDOFF.md` unless the human requests it.

