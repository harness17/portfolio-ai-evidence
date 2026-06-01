# Claude Code Handoff

## Project

Public software development portfolio for job-hunting and interview use.

Public site:
https://harness17.github.io/portfolio-ai-evidence/

Repository:
https://github.com/harness17/portfolio-ai-evidence

## Current Design Line

This site is a public one-page development portfolio. It should show public technical evidence only.

Positioning: lead with technical skills and shipped deliverables. AI-assisted workflow is one supporting element (the AIハーネス card + one talk-track item), not the main framing.

Core cards, in this order:

- YouTom
- DevNext
- AIハーネス

Each card uses the five fields: 課題, 自分の判断, 使用技術, 検証方法, 成果. ("AI委譲範囲" was replaced by "使用技術" on 2026-06-01 to foreground technical stack.)

Chrome extensions are listed as external proof, not as core cards. Both the Chrome Web Store link and the source repository (now split into independent repos) are linked.

## Privacy Boundary

Do not add private job-search documents, application tracking, email analysis, health details, contact details, addresses, phone numbers, or unpublished client/support-site details.

Do not add unpublished DevNext-based app details until the user confirms they are public. When permission is granted, rewrite the DevNext card in the context of "built using DevNext" rather than adding a separate private-project card.

## Collaboration Rules

- Read `git status` before editing.
- Keep changes scoped to `index.html`, `assets/styles.css`, `README.md`, or this handoff unless the user asks otherwise.
- Preserve the three-card structure (order: YouTom, DevNext, AIハーネス) unless the user explicitly changes the positioning.
- For each card, keep the same five fields: 課題, 自分の判断, 使用技術, 検証方法, 成果.
- Treat Chrome Web Store links as external proof; source repositories may be linked alongside them.

## Current Status

- 2026-06-01: Repositioned from "AI evidence map" to a job-hunting software development portfolio. Technical skills and shipped deliverables now lead; AI usage is demoted to one card and one talk-track item.
- Hero copy, title, meta description, and signal-board rewritten (signal-board now: 公開プロダクト 5+ / YouTom 115 DL / 公開技術記事 13+).
- Card order changed to YouTom → DevNext → AIハーネス. The "AI委譲範囲" field was replaced by "使用技術" in every card.
- talk-track rewritten so the 採用担当者 column leads with shipped products and stack; AI workflow is one item under 技術担当者.
- Chrome拡張 external-proof section now links both the Chrome Web Store entry and the independent source repos (youtube-playlist-date-sorter, amazon-wishlist-sale-picker).
- GitHub repo `harness17/google-chrome-extensions` archived (the two extensions now live in their own repos).

## Next Actions

- When the unpublished DevNext-based app can be public, revise DevNext to explain that the app was built using DevNext.
- Keep the public page concise enough to scan in about three minutes.
