# AGENTS.md

This is a public software development portfolio repository.

Before editing, read `CLAUDE_CODE_HANDOFF.md`.

## Rules

- Keep the page public-safe. Use the handle `harness` only — no real name, contact, address, health, or job-search details.
- Do not add private job-search documents, application tracking, email analysis, health details, contact details, or unpublished app details.
- Exception (approved 2026-07-31): one LAPRAS profile link in the hero button row is allowed as the recruiter-facing route. Do not extend this to email addresses, contact forms, 「転職活動中」 statements, or 職務経歴書請求 wording.
- The page targets 正社員・中途採用 for .NET/Web development. Lead with the ~9 years of professional experience, then the shipped personal products as evidence.
- Facts must match the private job-search records (resume). Web development is ~9 years, but C#／ASP.NET MVC is only ~4年8ヶ月 (the 2nd company); the 1st company was all Classic ASP. Never write that C# was used for 9 years. Never call the previous employer an 「ITコンサルティング企業」.
- Article counts: write Zenn and Qiita separately (Qiita includes reworked reposts of Zenn articles). Never sum them into one figure.
- DevNext wording: Claude Code was used to move the common base to the ASP.NET Core 10 structure, to see how it changes from .NET Framework 4.6.1. Do not say 「作り直した」 or 「一から再構築」. Never name or link the old template (DevNet).
- Lead with technical skills and shipped deliverables. AI-assisted workflow is one section ("開発の進め方 / How I work"), not a product.
- Section model, in this order: Hero → 強み → 業務経験（年数表 + 実務エピソード4件）→ 技術スタック・資格 → 実働プロダクト → 開発ベースの再構築 → 開発の進め方 → これから取り組みたいこと → Writing.
- 実務エピソード uses the same 課題 / 判断 / 結果 card shape as the product cards. Never invent metrics or episodes — the source is the user's own account, and no numbers were available.
- 実働プロダクト = shipped products, in this card order: Kototsubo, Phycock, YouTom, YouTube Playlist Date Sorter, Amazon Wishlist Sale Picker, Kindle Series Sale Tracker. Each product card uses 課題 / 役割 / 使用技術 / 成果 + links.
- DevNext belongs in 開発ベースの再構築 (not a product card). The AI harness (cross-agent-harness) belongs in 開発の進め方. Keep the link from the 開発標準 episode to `#foundation` — it is what connects the previous job to the current personal work.
- Treat Chrome Web Store links as external proof; source repositories may be linked alongside them.
- Keep the nav anchors (`#about`, `#experience`, `#projects`, `#approach`, `#interests`, `#writing`) in sync with the section ids. `#foundation` is a section id with no nav entry, by design — it is reached from the 開発標準 episode link.
- Check `git status` before editing and avoid overwriting changes from another agent.
