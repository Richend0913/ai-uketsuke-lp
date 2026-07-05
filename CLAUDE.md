# ai-uketsuke-lp

- **これは何**: L1「AI受付付きホームページ」事業の宣伝LP（BURNING STACK L1・層カラー=緑 #0e7c66）。静的HTML1枚。
- **本番URL**: https://richend0913.github.io/ai-uketsuke-lp/
- **デプロイ**: GitHub Pages（リポジトリ Richend0913/ai-uketsuke-lp）。`git push origin master` で自動反映（数分かかる）。wrangler/Cloudflareは使わない。
- **触ってはいけないもの**:
  - 価格表記（モニター月4,980／標準 初期15万+月9,800／プロ 初期30万+月14,800・すべて税込表示）は next-growth-ops スキルの価格正本と一致させること。勝手に変えない。
  - 正直設計: 実績・レビュー・法人格・代表者名・番地の捏造禁止。保証表現（「必ず」「絶対」「取りこぼしません」等）禁止。
  - AI受付widget（body末尾の widget.js script タグ）: data-site="ai-uketsuke-lp" のKV設定は genba-ai-core 側（Cloudflare アカウントB）が正本。widgetのFAB位置調整は `::part(fab)` のCSSで行う（Shadow DOMはclosed）。
  - GA4測定ID G-63VB4HT3T2 は head 内の1箇所のみ（TODOコメント付き）。差し替えはそこだけ。
- **修正時に読むスキル**: next-growth-ops → burning-lp → ai-employee-site の references/design-system.md（組版・禁止リスト）。
- **品質ゲート**: visual-qa スキルで 375px viewport スクショ確認（full-pageでなく実機viewport）。見出しの泣き別れ・固定バーとFABの重なり・console error ゼロを確認してからpush。デプロイ後に本番URLでもう1周。
