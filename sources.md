# 調査ソース

確認日: 2026年9月4日

出典は原則として Anthropic の公式ドキュメント。Claude Code は更新頻度が高いため、参照する前にリンク先の現在の内容を確認するとよい。

## 主要ソース

1. [Manage costs effectively](https://code.claude.com/docs/en/costs)
   - `/usage`、`/clear`、`/compact`、モデル選択、MCP、`CLAUDE.md`、thinking、エージェントチームのコスト管理
2. [Best practices for Claude Code](https://code.claude.com/docs/en/best-practices)
   - コンテキスト管理、具体的な依頼、`/btw`、サブエージェント、修正ループからの再開
3. [Explore the context window](https://code.claude.com/docs/en/context-window)
   - 起動時と作業中に読み込まれる情報、圧縮後に残る情報、`/clear` と `/compact`
4. [Manage sessions](https://code.claude.com/docs/en/sessions)
   - `/clear`、`/compact`、`/context`、セッションの再開と保存
5. [How Claude remembers your project](https://code.claude.com/docs/en/memory)
   - `CLAUDE.md`、path-scoped rules、auto memory、200行の目安
6. [Customize your status line](https://code.claude.com/docs/en/statusline)
   - コンテキスト使用率とコストの表示、ステータスラインがAPIトークンを使わないこと
7. [Model configuration](https://code.claude.com/docs/en/model-config)
   - モデル選択、effort、extended thinking、`opusplan`、拡張コンテキスト
8. [Create custom subagents](https://code.claude.com/docs/en/sub-agents)
   - サブエージェントの独立コンテキスト、適した用途、返答がメインのコンテキストへ与える影響
9. [Extend Claude Code](https://code.claude.com/docs/en/features-overview)
   - `CLAUDE.md`、スキル、MCP、サブエージェントなどのロード時期とコンテキストコスト
10. [Monitoring](https://code.claude.com/docs/en/monitoring-usage)
    - OpenTelemetry のトークン・コスト・モデル・effort 関連メトリクス
11. [Commands](https://code.claude.com/docs/en/commands)
    - `/usage`、`/cost`、`/context`、`/clear`、`/compact` などのコマンド一覧

## 解釈上の注意

- 公式資料の「コスト」は、APIの金額課金とサブスクリプションの利用枠の両方を指す。このガイドでは、両者に共通する改善策を「トークン節約」と呼んでいる。
- チェックリストの項目立て、推奨する着手順、効果の確かめ方は、このガイド独自の整理であり、Anthropic の公式基準ではない。
- モデル名、利用可能な effort、既定値、料金、コマンドの挙動は変わりうる。ここに書かれた固定値を前提にする場合は、その時点の公式資料で確認する。
