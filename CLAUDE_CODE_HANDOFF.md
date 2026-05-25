# Claude Code Handoff

## Project

AI Evidence Map for portfolio and interview use.

Public site:
https://harness17.github.io/portfolio-ai-evidence/

Repository:
https://github.com/harness17/portfolio-ai-evidence

## Current Design Line

This site is a public one-page evidence map. It should show public technical evidence only.

Core cards:

- AIハーネス
- YouTom
- DevNext

Chrome extensions are listed as external proof, not as core cards.

## Privacy Boundary

Do not add private job-search documents, application tracking, email analysis, health details, contact details, addresses, phone numbers, or unpublished client/support-site details.

Do not add unpublished DevNext-based app details until the user confirms they are public. When permission is granted, rewrite the DevNext card in the context of "built using DevNext" rather than adding a separate private-project card.

## Collaboration Rules

- Read `git status` before editing.
- Keep changes scoped to `index.html`, `assets/styles.css`, `README.md`, or this handoff unless the user asks otherwise.
- Preserve the three-card structure unless the user explicitly changes the positioning.
- For each card, keep the same five fields: 課題, 自分の判断, AI委譲範囲, 検証方法, 成果.
- Treat Chrome Web Store links as external proof.

## Current Status

- AIハーネス card has been rewritten from user hearing.
- YouTom card has been rewritten from user hearing.
- DevNext card has been rewritten from user hearing.
- Chrome Web Store links are present for YouTube Playlist Date Sorter and Amazon Wishlist Sale Picker.
- External proof section is grouped by project: AIハーネス, YouTom, DevNext, Chrome拡張.
- Public repository links and Zenn/Qiita article links have been added and checked for HTTP 200.
- note profile is linked from the hero actions and external proof section.

## Next Actions

- Review whether each card avoids overstating AI delegation.
- When the unpublished DevNext-based app can be public, revise DevNext to explain that the app was built using DevNext.
- Keep the public page concise enough to scan in about three minutes.
