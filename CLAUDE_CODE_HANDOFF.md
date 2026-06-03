# Claude Code Handoff

## Project

Public software development portfolio for job-hunting and interview use.

Public site:
https://harness17.github.io/portfolio-ai-evidence/

Repository:
https://github.com/harness17/portfolio-ai-evidence

## Current Design Line

This site is a public one-page software development portfolio. It should show public technical evidence only.

Positioning: lead with technical skills and shipped deliverables. AI-assisted workflow is one section ("開発の進め方 / How I work"), not a product.

Section model, in order (rebuilt 2026-06-01, experience added 2026-06-03):

1. Hero — handle, role, value line, links, three headline metrics (実働プロダクト 3 / 技術記事 13+ / 公開リポジトリ 8+).
2. About / 強み — short self-intro + three strength panels.
3. 業務経験 — professional background from ~9 years of web 受託開発. Three panels aligned with the resume: 業種知識 (コーポレートサイト/旅行予約/コンベンション/EC/官公庁), 経験フェーズ (要件定義〜運用改善), 環境・ミドルウェア (Windows Server/SQL Server/IIS/サイボウズ/Redmine). Lead mentions PL leader experience (max 4 members). Items and labels must match the resume (職務経歴書).
4. 技術スタック — two provenance blocks: 実業務で使用 (前職での経験: C#/ASP.NET MVC/ASP Classic/SQL/JavaScript/jQuery/HTML・CSS/SVN) and 個人開発で習得 (ASP.NET Core/Identity/EF Core/React/Electron/YouTube Data API/OAuth/Chrome Extensions/Git/GitHub Actions/Claude Code/Codex), as tag chips. Note: version control split — SVN was the work tool, Git is personal-dev. Do not merge back into one block — the split shows professional depth vs. self-driven learning.
5. 実働プロダクト — shipped products: YouTom, YouTube Playlist Date Sorter, Amazon Wishlist Sale Picker. Each card uses 課題 / 役割 / 使用技術 / 成果 + links.
6. エンジニアリングの土台 — DevNext (ASP.NET Core). Not a product card.
7. 開発の進め方 — the AI harness (cross-agent-harness), handoff contracts, review gate, skill化. This is where AI usage lives.
8. Writing — six curated articles + links to full Zenn/Qiita/note.

Nav anchors: `#about`, `#experience`, `#projects`, `#approach`, `#writing` — keep in sync with section ids.

Chrome extensions are shipped products in 実働プロダクト. Their Chrome Web Store link and source repo are both linked. Install counts are intentionally omitted (they undersell). No product screenshots (they leak personal data: subscriptions, wishlist items).

## Privacy Boundary

Do not add private job-search documents, application tracking, email analysis, health details, contact details, addresses, phone numbers, or unpublished client/support-site details.

Do not add unpublished DevNext-based app details until the user confirms they are public. When permission is granted, rewrite the DevNext card in the context of "built using DevNext" rather than adding a separate private-project card.

## Collaboration Rules

- Read `git status` before editing.
- Keep changes scoped to `index.html`, `assets/styles.css`, `README.md`, or this handoff unless the user asks otherwise.
- Follow the seven-section model in Current Design Line. Do not collapse it back into uniform 5-field cards.
- Keep AI usage confined to the 開発の進め方 section; do not promote it to a product.
- Treat Chrome Web Store links as external proof; source repositories may be linked alongside them.
- Use the handle `harness` only; never add a real name or contact details.

## Current Status

- 2026-06-03: Added 業務経験 section (between About and Tech Stack) with Doda-sourced professional data: 案件領域 (7 items), 開発フェーズ (7 items), 環境・ミドルウェア (4 items), each with year indicators. Added ASP Classic to 実業務 tech tags. Nav updated with #experience. Section model now 8 sections.
- 2026-06-01 (structural rebuild): Rebuilt the whole page from the old "3 cards × 5 fields + wall-of-links proof + HR/tech talk-track" into the seven-section model above. Added About/強み and 技術スタック (previously missing). Promoted the two Chrome extensions to 実働プロダクト alongside YouTom. Moved DevNext to エンジニアリングの土台 and the AI harness to 開発の進め方. Dissolved the talk-track section into About + 開発の進め方. Curated Writing down to six articles. `styles.css` extended (additive) with .panel/.strengths/.skill-groups/.tags/.project-links/.foundation-grid/.approach-grid/.writing-grid. Nav re-pointed to #about/#projects/#approach/#writing. Verified on desktop and 375px; all nav anchors resolve; no real name present.
- 2026-06-01: Repositioned from "AI evidence map" to a job-hunting software development portfolio. Technical skills and shipped deliverables now lead; AI usage is demoted to one card and one talk-track item.
- Hero copy, title, meta description, and signal-board rewritten (signal-board now: 公開プロダクト 5+ / YouTom 115 DL / 公開技術記事 13+).
- Card order changed to YouTom → DevNext → AIハーネス. The "AI委譲範囲" field was replaced by "使用技術" in every card.
- talk-track rewritten so the 採用担当者 column leads with shipped products and stack; AI workflow is one item under 技術担当者.
- Chrome拡張 external-proof section now links both the Chrome Web Store entry and the independent source repos (youtube-playlist-date-sorter, amazon-wishlist-sale-picker).
- GitHub repo `harness17/google-chrome-extensions` archived (the two extensions now live in their own repos).

## Next Actions

- When the unpublished DevNext-based app can be public, revise DevNext to explain that the app was built using DevNext.
- Keep the public page concise enough to scan in about three minutes.
