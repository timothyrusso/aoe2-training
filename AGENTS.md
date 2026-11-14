# Agent Guidelines

## Project purpose

This repository contains a lightweight, static, in-game training guide for **Age of Empires II: Definitive Edition**.

Its primary goal is to help players make quick decisions during matches, with:
- a step-by-step Bohemians build order for Black Forest;
- economy, buildings, technologies, and military production guidance;
- searchable enemy-unit counters, including unique units;
- advice tailored to team games against AI.

The guide is designed to be consulted **while playing**, not read like a wiki.

## Files and deployment

- `index.html` is the main application, with self-contained HTML, CSS, and JavaScript.
- `README.md` contains the repository overview.
- GitHub Pages publishes `index.html` from the repository's `main` branch.
- Keep the page usable without a backend, build step, or external runtime dependencies.

## Design priorities

1. **Immediate readability:** short action-oriented bullet points, prominent timings, compact labels, consistent spacing, and legible text.
2. **Low interaction cost:** do not add checklists, timers, exports, or other controls that distract during gameplay unless explicitly requested.
3. **Clear layout:** keep the build/execution order on the left and the searchable unit-counter reference on the right on wide screens; stack them responsively on small screens.
4. **Concrete guidance:** state exact villager allocations, units, quantities, buildings, technologies, and prerequisites where justified. Avoid duplicating information already shown in timing labels.
5. **Accuracy:** distinguish tested game mechanics from estimated build timings or tactical advice. Do not imply a strategy guarantees victory.

## Content and data

- User-facing text should be in **Italian**. This file is in English for future agents.
- Default scenario: **Bohemians**, **large Black Forest**, **three human players versus two Hard AI**, **500 population cap**.
- Keep the guide adaptable to map variations (for example, distant or different huntable animals) and enemy compositions.
- When updating unit counters, verify the currently available civilizations, DLC units, Bohemian tech-tree availability, production buildings, and relevant patch changes.
- Avoid generic counters when unique armor classes, bonuses, range, or mobility materially change the matchup.
- Keep combat recommendations concise enough to scan mid-match.

## Editing and validation

- Prefer small, focused edits rather than wholesale rewrites.
- Preserve existing responsive behavior, search/filter controls, and GitHub Pages compatibility.
- Check HTML nesting and closing tags when moving sections.
- Validate JavaScript syntax and test visible rendering at desktop and mobile widths when possible.
- Watch for horizontal overflow, broken padding, excessively wrapped timing labels, and missing build steps.
- Do not introduce heavy frameworks or dependencies without a clear benefit.
- Make changes directly to `main` only when the user requests publishing; otherwise use an appropriate branch and pull request.

## Project boundaries

This is a practical training reference, **not** a comprehensive AoE II wiki, an automated victory predictor, or a general-purpose analytics platform. New features should improve speed, clarity, or usefulness during actual matches.
