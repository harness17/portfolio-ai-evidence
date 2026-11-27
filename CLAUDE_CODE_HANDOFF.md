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

Section model, in order (rebuilt 2026-06-01, experience added 2026-06-03, synced with the page 2026-11-24). `CLAUDE.md` holds the short version; keep both in sync:

1. Hero — handle, role, value line, links, three headline metrics (業務開発経験 9年 / 公開プロダクト 6 / Zenn技術記事 38). Never sum Zenn and Qiita counts.
2. About / 強み — short self-intro + three strength panels. The first panel is the work-derived strength (要件から運用まで一貫・代案で合意・リーダー最大4名); the second merges shipping and writing (YouTom・拡張・Zenn 38／Qiita 57); the third is AI. Do not move the work panel behind the personal-dev ones (2026-11-26).
3. 業務経験 — professional background from ~9 years of web development at two companies (1st: Classic ASP, 2nd: C#／ASP.NET MVC ~4年8ヶ月). Below the panels: 実務エピソード6件 (6th added 2026-11-26: 演題処理システムの自由設問フォームの共通化) (the 5th, Redmine導入, was added 2026-11-26 from the user's own account; it is the 社内SE-facing episode) (課題 / 判断 / 結果). Three panels aligned with the resume: 業種知識 (公営競技サイト（自治体施行）/旅行予約/コンベンション/コーポレート・社内システム), 経験フェーズ (要件定義〜運用改善), 環境・ミドルウェア (Windows Server/SQL Server/IIS/サイボウズ/Redmine). Lead mentions PL leader experience (max 4 members). Items and labels must match the resume (職務経歴書). 業種知識 was corrected 2026-08-21: the year figures originally came from a doda skill sheet, not the resume — the resume lists the industries without years. Each remaining row must trace to a resume project (公営競技=トランスワード期のボートレース場サイト 4年5ヶ月, 旅行予約=2017/9-2019/9, コンベンション=2019/10-2021/3). 「官公庁」was renamed because the actual work is 公営競技場のサイト・管理画面 and the old label implied 中央省庁/自治体基幹系. ECサイト was dropped — no project in the resume backs it. コーポレート uses 「複数案件」 instead of a year figure because the resume only says 「複数担当（各案件2〜3ヶ月サイクル）」. 経験フェーズ and 環境 were corrected the same day, same reason: the resume carries a year figure for exactly one row (SQL Server 5年以上) and the rest were doda values. 経験フェーズ is now the sum of the resume's per-project 担当フェーズ (要件定義/基本設計 3年9ヶ月 = 旅行予約2年 + 演題1年半 + 下関3ヶ月; 詳細設計 3年6ヶ月 = 下関 lists no 詳細設計; 実装/テスト 約9年 = both tenures; 運用改善 4年 = トランスワード期の改修案件). 環境: Windows Server/SQL Server/IIS 約9年 (both tenures' 開発環境), サイボウズ 4年8ヶ月 and Backlog 3年6ヶ月 (旅行予約 + 演題) came from the user directly — neither is in the resume. Redmine is 1年4ヶ月 (2016/5 導入〜2017/8 退社), not the 導入3ヶ月 the resume's project entry implies. Do not reintroduce year figures that cannot be traced to a project period.
4. 技術スタック・資格 — a 資格 panel (取得年月) plus two provenance blocks: 実業務で使用 (前職での経験: C#/ASP.NET MVC/Entity Framework/ASP.NET Identity/Classic ASP（VBScript）/SQL Server/JavaScript/jQuery/Ajax/HTML・CSS/Bootstrap/AutoMapper/EPPlus/Microsoft.Reporting/log4net/SVN) and 個人開発で使用 (ASP.NET Core/Identity/EF Core/React/Electron/YouTube Data API/OAuth/Chrome Extensions/Git/GitHub Actions/Claude Code/Codex), as tag chips. Note: version control split — SVN was the work tool, Git is personal-dev. Do not merge back into one block — the split shows professional depth vs. self-driven learning.
5. 実働プロダクト — shipped products, in this card order: Kototsubo, Phycock, YouTom, YouTube Playlist Date Sorter, Amazon Wishlist Sale Picker, Kindle Series Sale Tracker. Each card uses 課題 / 役割 / 使用技術 / 成果 + links.
6. 開発ベースの再構築 (`#foundation`) — DevNext (ASP.NET Core). Not a product card. Reached from the 開発標準 episode link.
7. 開発の進め方 — the AI harness (cross-agent-harness), handoff contracts, review gate, skill化. This is where AI usage lives.
8. これから取り組みたいこと (`#interests`).
9. Writing — six curated articles + links to full Zenn/Qiita/note.

Nav anchors: `#about`, `#experience`, `#projects`, `#approach`, `#interests`, `#writing` — keep in sync with section ids. `#foundation` has no nav entry by design.

Chrome extensions are shipped products in 実働プロダクト. Their Chrome Web Store link and source repo are both linked. Install counts are intentionally omitted (they undersell). No product screenshots (they leak personal data: subscriptions, wishlist items).

Kototsubo privacy rule: describe the media types it handles (本・ゲーム・映像作品・音楽CD) and its features, as listed in the public README. Do not mention specific personal collection contents (titles the user owns).

## Privacy Boundary

Do not add private job-search documents, application tracking, email analysis, health details, contact details, addresses, phone numbers, or unpublished client/support-site details.

Do not add unpublished DevNext-based app details until the user confirms they are public. When permission is granted, rewrite the DevNext card in the context of "built using DevNext" rather than adding a separate private-project card.

## Collaboration Rules

- Read `git status` before editing.
- Keep changes scoped to `index.html`, `assets/styles.css`, `README.md`, or this handoff unless the user asks otherwise.
- Follow the section model in Current Design Line. Do not collapse it back into uniform 5-field cards.
- Keep AI usage confined to the 開発の進め方 section; do not promote it to a product.
- Treat Chrome Web Store links as external proof; source repositories may be linked alongside them.
- Use the handle `harness` only; never add a real name or contact details.

## Current Status

- 2026-11-27: 技術スタックの「個人開発で習得」を「個人開発で使用」に改め、補足を「Claude Code・Codex と組んで開発し、設計判断とレビューは自分で行った技術」にした（本人決定）。実装は主に AI に任せている（バイブコーディング）ため「習得」は言い過ぎで、面接で深く聞かれたときに詰まる元になるため。以後「習得」は使わない。
- 2026-11-27: 業務経験の冒頭の文を、エピソードへの案内に書き換えた（「要件定義〜テストを一貫・最大4名」がヒーロー・強み・業務経験で3回続いていたため）。C# の年数を分ける書き方は維持。
- 2026-11-27: 「個人開発で習得」に xUnit / jsdom / SQLite を追加（カードと検証のしかたに出ているのにタグになかったため）。リンクの共有プレビュー用に OGP と twitter:card を追加（画像はワークフロー図）。README の説明を今の構成（業務経験が先）に合わせた。Zenn の本数（38）は、この環境から Zenn を開けず API では数え直せていないが、2026-11-27 に本人から「追加公開していない」と確認済み。
- 2026-11-26: これから取り組みたいことを見直し（本人が案A・Cを選択）。「現場の手間を減らす業務改善」（前職のRedmine導入・自由設問フォームを根拠に、使う人の話から入り運用側が自分で回せる形にする）と「社内でAIを使う仕組みづくり」（個人のハーネスと生成AIパスポートの知識を、社内で安全に使うルールづくり・チームの進め方へ）の2項目に差し替え。旧「AIを組み込んだ開発プロセスの整備」「本質的に役に立つ業務改善プロダクトの開発」は廃止。案B（古いシステムを新しい .NET へ移す）は本人が選ばなかった。
- 2026-11-26: 検証のしかたの「dotnet test / npm test」が端的すぎたため、「変更の種類ごとに回すテストを決めておき、完了前に必ず実行する（ASP.NET Core は dotnet test、拡張と Electron アプリは npm test）」に書き直し。出典は「cross-agent-harnessのverifyを変更種別と作業ルートで分岐するのは誤検証を防ぐため」。
- 2026-11-26: 開発の進め方を膨らませた。パネルを4枚に（自分で決めること／AIの役割分担（新規）／仕組み化していること／検証のしかた）。出典はすべて My-Skill-Graph の判断記録：AIの役割分担＝「Codex実装委譲でcommitさせないのはレビュー責任をClaudeCode側に残すため」「ClaudeCode自動呼び出しをレビュー専用から始めるのは上書き事故を避けるため」「CodexとClaudeの協調をhandoffで管理するのは編集衝突を避けるため」。自分で決めることの守秘の例＝「Kototsuboを公開専用ルートコミットから配布したのは秘密を含む履歴を公開しないため」。検証＝「DOM変更で壊れる検出ロジックはjsdomとフィクスチャでリグレッション検証する」「DevNextのmaster反映をPRとCI必須にしたのはローカル検証の抜けを防ぐため」。
- 2026-11-26: 実務エピソード6件を面接での有効度順に並べ替え（本人依頼）：自由設問フォームの共通化 → Redmine導入 → 共通ライブラリとひな形 → プラン設定の整合性チェック → 地域の選択肢の代案 → 申込一覧の表示遅延。順番の考え方：設計判断と運用側への効果が両方ある話を先に、社内SE向けの主体性、標準化とDevNextへの接続、運用の問い合わせ削減、顧客折衝、一般的な性能改善の順。
- 2026-11-26: 開発の進め方の「仕組み化していること」に My-Skill-Graph（設計判断のナレッジグラフ、判断記録270件超＝2026-11-26 時点で decisions/ の index を除く276件）を追加。リポジトリは private なのでリンクは貼らない。ワークフロー図の alt には以前から名前が出ていた。
- 2026-11-26: 業務経験の「経験フェーズ」を、要件定義〜テスト 約9年／運用改善 4年の2行と注記「2社とも、案件ごとに要件定義・基本設計・詳細設計・実装・テストまで一貫して担当」にまとめた（本人決定）。本人確認：トランスワードでは入社から退社まで要件定義・基本設計・詳細設計を担当、プロアクティブでも旅行予約・演題処理以外の MICE 案件で要件定義をしていた。職務経歴書の両社の担当業務「要件定義〜テスト」とも一致。これにより、以前の「経験フェーズはプロジェクト欄の担当フェーズの合計（要件定義・基本設計 3年9ヶ月、詳細設計 3年6ヶ月）」という数え方は廃止。パネルが短くなったため「プログラマリーダー 最大4名」（演題処理システム）の行を足した（本人決定）。
- 2026-11-26: 実務エピソードの6件目「学会ごとに違う設問を、開発なしで設定できるフォーム設計に」（設計 · 共通化）を追加。中身はすべて本人の聞き取り：演題処理システムで、旅行予約システム（別担当が開発）のような自由設問を3フォームに入れる要望。旅行予約版はフォームの型がなくHTMLと表示タグを書く必要があり、運用側で扱えず開発へ手戻り、細かなカスタマイズ・修正・新規登録が多かった。3フォームの仕様を共通化して設計（フォーム→自由/基本設問→小項目、基本回答→自由設問回答に設問・小項目をJoinして再現）、フォームごとに3種用意。連動設問は表示制御を汎用JS関数にして動的に。結果：学会ごとの設問差を開発なしで管理画面から設定、3フォームを同じ仕組みで保守、メンテナンスコストを大きく下げた。3フォームは演題投稿・査読・講演者登録（本人の記憶ベースで「だったかな」）。ページには書かない（本人と相談して、なくても伝わるため）。面接で聞かれたら答える材料。
- 2026-11-26: 実働プロダクトの判断欄・使用技術を My-Skill-Graph の判断記録と突き合わせて見直し。YouTom：判断を「RSS主経路＋失敗時のみAPI、切り替えにチャンネル単位クールダウンと更新ごとの上限、通常時は1日約200ユニット」に具体化（出典「RSSハイブリッド取得で…」「RSS失敗時のAPIフォールバックを制限した…」）、使用技術に SQLite（better-sqlite3）と OAuth 2.0（プレイリスト同期）を追加。YouTube Playlist Date Sorter：判断に「再描画でDOM順が戻るためCSS orderで固定」「MutationObserverは行構造の変化だけ監視」を追加。Kindle Series Sale Tracker：使用技術の LocalStorage を chrome.storage / Side Panel API に訂正（蔵書は拡張の storage quota 対策で圧縮保存、UIはサイドパネル）、判断を「判別不能は前回結果を保持、3シリーズ連続で実行全体を失敗にして再試行」に具体化。Kototsubo・Phycock・Wishlist は今のままで記録と一致。
- 2026-11-26: Amazon Wishlist Sale Picker のカードに判断欄を追加（6枚すべてに判断欄がそろった）。出典は本人の My-Skill-Graph の判断記録（private）：「欲しいものリストの全件読み込みを終端マーカーで止めるのは取りこぼしを防ぐため」（v0.5.2、368件中290件の事象）、「lazy-load対応で固定待機ではなくMutationObserver駆動の動的待機を選んだ…」、「横断セールスキャンをタブ順次方式にした…」（v0.4.0、成果欄に横断セール確認を追加）。使用技術に MutationObserver を追加。
- 2026-11-26: 資格パネルに生成AIパスポート（2026年9月）を追加（情報セキュリティマネジメントは掲載済み）。Phycock の成果欄を就活側の職務経歴書の言い方（「Phase 1（MVP）まで実装して、開発を終えました」、2026-11-21 本人確認：開発は終了、公開サイトは残す）に合わせ、「Phase 1（MVP）まで実装して開発を完了。…Azure上のサンプルサイトとGitHubで公開を続けている」にした。
- 2026-11-26: 「パフォーマンス改善」エピソードを具体化（本人の言葉）：旅行予約システムの申込一覧画面。申込内容を表示する列があり、対象プランを施設ごとに1件ずつ取得していたので、まとめて連結して取得するように変えた。見出しを「申込一覧の表示の遅れを、データの取り方の見直しで解消」にし、課題と判断に場面を入れた。結果欄は元の文のまま。要件定義エピソードの判断は本人の言い方（「別口で設定しなければいけない内容だった」）に合わせた。これで実務エピソード5件がすべて具体的な場面を持つ形になった。判断欄にテーブルの階層（申込 → 施設 → プランごとの申込情報 → プラン）を追加。本人の記憶ベース（「確か」）で、在籍時の資料では確認できない。
- 2026-11-26: 「要件定義・顧客折衝」エピソードを具体化するため聞き取り中（本人の言葉）：旅行予約システムの利用者側の検索画面。フラグのチェックで足りる項目をセレクトボックスに入れるよう指示が出ていたため、折衝してチェックボックスにした（本人訂正：ラジオボタンではなくチェックボックス）。詳しくは、地域のセレクトボックスの中に、別項目としてフラグチェックで絞り込んでいた条件を入れようとしていた。カードの見出し・課題・判断をこの内容で書き直した。「地域とその条件を同時に指定できなくなる」は単一選択のセレクトボックスに入れた場合の帰結として書いた。結果欄（合意して仕様確定・要件定義から実装設計まで担当）は元の文のまま。
- 2026-11-26: 「開発標準の策定」エピソードを具体化。見出しを「共通ライブラリとひな形を整え、社内の新規開発案件4件の標準に」にし、判断に中身（旅行予約システムから汎用部品を抜き出して土台に／エンティティ・リポジトリ基底クラスでDB・CRUD共通化／PDF・Excel出力・ファイル取込・バッチのサンプル／Bootstrapで管理画面を統一しページャー等を共通化／案件で必要になった機能を切り出して取り込み）、結果に「演題処理システムを含む新規開発案件4件で標準」「当初から実質的に担当、2020年9月から取りまとめ」を入れた。出典は就活リポジトリの引き継ぎ資料と職務経歴書の追記案（2026-11-13・11-19 本人確認）。旧テンプレートの名前は出さない。`#foundation` へのリンクは維持。
- 2026-11-26: 「入力ミスの削減」エピソードを具体化するため聞き取り中（本人の言葉）。入力ミス＝管理者が宿泊プランを設定するときに、販売期間と公開期間の組み合わせを間違える。困りごと＝運用担当者から「プランが表示されない」「申し込みができない」という問い合わせが定期的に来ていた。判断＝保存時に販売期間が公開期間からはみ出していればエラーにした。施設情報とプラン情報が矛盾しないかのチェックも入れた。結果＝問い合わせがほぼ来なくなった。これでカードを書き直した（見出し「「プランが表示されない」問い合わせを、設定時の整合性チェックでなくす」）。
- 2026-11-26: ポートフォリオ見直し（本人決定）。(1) 強みの1枚目を業務由来の「要件から運用まで一貫して担う」に差し替え、「作って公開し切る」「書いて言語化する」を「作って公開し、書いて残す」の1枚にまとめた。採用側が最初に見る場所で仕事としての経験が伝わるようにするため。(2) Phycock のカードに運用の判断を追加：Azure SQL の自動休止からの復帰時に起動が失敗する事象を Kudu のイベントログ（エラー40613）で特定し、EF Core の接続再試行設定で解消（就活側の職務経歴書8月更新案・面接想定QA と同じ事実）。役割に「運用」、使用技術に Azure App Service / Azure SQL Database、成果に「Azure公開」を追加。(3) カード順を Kototsubo → Phycock に入れ替え（連携APIが最も多く、6本の中で一番重い作品のため）。(4) 業務経験に5件目のエピソード「散らばっていた部内の案件管理を、Redmineの導入で見える化」（社内改善 · ツール導入）を追加。トランスワード期・2016/5〜2017/8。社内SE向けの裏付け。中身はすべて本人の聞き取り（2026-11-26）：課題＝部署内の案件管理をメールや Skype で行い、各人のタスクや問い合わせが散らばって判断が難しく、担当状況も把握できていなかった。判断＝無料で社内に置け、よく知られたツールなので Redmine を選定。余っていたPCで社内サーバーを立ち上げ、インストール・設定・ユーザー管理、プロジェクト／タスク管理とチケットの切り方のルール決めと説明まで一人で行った。結果＝プロジェクト単位で管理できるようになり、部署内で何をしているか・業務の大枠が見えるようになった。各人のタスク量が把握でき部内の連絡がスムーズになった。個人でも受け持ちやタスクの受け渡しが分かり仕事が進めやすくなった（本人：「かなり快適にタスク管理できた」）。数字はない。社内SE向けの話が最初に目に入るよう、エピソードの先頭に置いた（本人決定）。
- 2026-11-24: 「実業務で使用」を8個から16個に増やした（本人決定）。根拠は2種類。(A) 経歴書・本人確認：Entity Framework（旅行予約・演題処理の開発環境）、Bootstrap（開発標準化で管理画面を Bootstrap 4 ベースに統一、2026-11-19 本人）、Ajax（経歴書の言語・FW欄）。表記を経歴書にそろえ「ASP Classic」→「Classic ASP（VBScript）」、「SQL / RDB」→「SQL Server」。(B) 開発標準化のひな形で使っていたライブラリ：ASP.NET Identity / AutoMapper / EPPlus / Microsoft.Reporting / log4net。B の根拠は削除前の旧テンプレートを 2026-11-13 に読んだ記録で、コードは削除済みのため再確認できない。旧テンプレートの名前は出さない。同時に「個人開発で習得」の「Identity」を「ASP.NET Core Identity」に改名（実務側の ASP.NET Identity と区別するため）。
- 2026-11-24: 就活リポジトリの最新の事実に合わせて修正。(1)「ITコンサルティング企業」を削除（実態はMICE支援会社で、書類・面接でも使わない表現）。(2) C#／ASP.NET MVC を9年と読める箇所（meta description・業務経験の冒頭の文）を「Web開発 約9年、うち C#／ASP.NET MVC 約4年8ヶ月」に分けた。1社目は全案件 Classic ASP。h1 も「業務系Webアプリを9年」→「Webアプリ開発を約9年」。(3) DevNext の説明を、就活側で決めた言い方（.NET Framework 4.6.1 から ASP.NET Core 10 でどう変わるかを確かめるため、Claude Code で共通基盤を移し替えた）にそろえた。「作り直した」「一から再構築」は使わない。開発標準エピソードの `#foundation` リンクは維持。(4) 記事数は合算しない（Qiita に Zenn 記事の改稿転載を含むため）。ヒーローの指標は「38 Zenn技術記事」、強みパネルは「Zennに38本、Qiitaに57本」。(5) ブラウザ拡張3本は Chrome・Firefox 両ストア公開に表記をそろえた。(6) 個人開発の技術に Azure App Service / Azure SQL Database / Playwright を追加。(7) 技術スタックの節を「技術スタック・資格」にし、資格パネル（情報セキュリティマネジメント 2026年11月／基本情報技術者 2011年11月）を足した。同日、Kototsubo のカードを公開 README に合わせて本・ゲーム・映像作品・音楽CDまで広げた（本人決定）。連携先は NDL Search / openBD / 楽天ブックスAPI / MADB / IGDB / Steam 一覧JSON。TypeScript は「個人開発で習得」から削除（公開リポジトリに TypeScript が主言語のものがなく、学習計画でも未着手のため。本人決定）。実際に使ったリポジトリができてから戻す。YouTom の最新版は v1.24.1（2026-06-13 リリース、タグとmasterで確認）でページの記載と一致。

- 2026-11-13: Zenn記事「ASP.NET Core移行でIdentityエンティティを共通化した判断」を非公開化したため、DevNextのプロジェクトリンクから外し、Writingカードを「自作HelperをASP.NET Coreに移植した」(devnext-mvc-helper-extensions) に差し替えた。旧テンプレートDevNetは削除済みで、ページでは名前もリンクも出さない。
- 2026-07-28: PhycockをAzureサンプルサイトとして公開。Kototsuboと同じく、プロダクトカードに「Azureサイト」と「ログイン情報などはGitHub参照」を追加した。資格情報はポートフォリオへ重複掲載せず、公開リポジトリのREADMEを正本とする。
- 2026-06-24: Updated metrics: YouTom v1.23.0→v1.24.1, DL 52→300超, 記事 40+→70+ (Zenn 31 + Qiita 41), リポジトリ 9+→13, プロダクト 5→6. Added Kototsubo (蔵書管理・言葉収集 Web app) as 6th product. Updated DevNext成果 to mention Kototsubo. Updated About panels (DL count, extension count 2→3, article count).
- 2026-06-05: Added Phycock (ASP.NET Core 10 MVC 体調管理 Web app) to 実働プロダクト. Updated YouTom to v1.23.0 (was v1.19.0). Updated article count to 40+ (Zenn 18 + Qiita 22, was 13+). Updated repo count to 9+. Updated signal board: 実働プロダクト 5 / 公開技術記事 40+ / 公開リポジトリ 9+. Updated DevNext 成果 to mention Phycock. Phycock card: 課題/役割/使用技術/成果 + GitHub + Zenn PDF article link.
- 2026-06-03: Added 業務経験 section (between About and Tech Stack) with Doda-sourced professional data: 案件領域 (7 items), 開発フェーズ (7 items), 環境・ミドルウェア (4 items), each with year indicators. Added ASP Classic to 実業務 tech tags. Nav updated with #experience. Section model now 8 sections.
- 2026-06-01 (structural rebuild): Rebuilt the whole page from the old "3 cards × 5 fields + wall-of-links proof + HR/tech talk-track" into the seven-section model above. Added About/強み and 技術スタック (previously missing). Promoted the two Chrome extensions to 実働プロダクト alongside YouTom. Moved DevNext to エンジニアリングの土台 and the AI harness to 開発の進め方. Dissolved the talk-track section into About + 開発の進め方. Curated Writing down to six articles. `styles.css` extended (additive) with .panel/.strengths/.skill-groups/.tags/.project-links/.foundation-grid/.approach-grid/.writing-grid. Nav re-pointed to #about/#projects/#approach/#writing. Verified on desktop and 375px; all nav anchors resolve; no real name present.
- 2026-06-01: Repositioned from "AI evidence map" to a job-hunting software development portfolio. Technical skills and shipped deliverables now lead; AI usage is demoted to one card and one talk-track item.
- Hero copy, title, meta description, and signal-board rewritten (signal-board now: 公開プロダクト 5+ / YouTom 115 DL / 公開技術記事 13+).
- Card order changed to YouTom → DevNext → AIハーネス. The "AI委譲範囲" field was replaced by "使用技術" in every card.
- talk-track rewritten so the 採用担当者 column leads with shipped products and stack; AI workflow is one item under 技術担当者.
- Chrome拡張 external-proof section now links both the Chrome Web Store entry and the independent source repos (youtube-playlist-date-sorter, amazon-wishlist-sale-picker).
- GitHub repo `harness17/google-chrome-extensions` archived (the two extensions now live in their own repos).

## Next Actions

- Keep the public page concise enough to scan in about three minutes.
- Phycock privacy rule: never mention health context, Ritalico, 就労移行支援, or 訓練. Generic "体調管理" description only.
