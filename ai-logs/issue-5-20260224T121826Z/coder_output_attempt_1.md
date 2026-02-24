Issue #5 向けに、要件仕様を最小変更で更新しました。

変更内容:
- 要件トレーサビリティ表を追加（Issue要求と `FR-01`〜`FR-04` を 1:1 対応）
- `FR-01` / `FR-03` / `FR-04` に「保存有無（副作用）」を明記
- `FR-03` に成功レスポンス例（`receptionId`, `processedAt`）を追加
- 処理順序を実装しやすい形に修正（API呼び出し時に10秒タイムアウト監視、成功確定条件を明確化）

変更ファイル:
- [ISSUE-0001-requirements.md](/home/runner/work/FlowSmith/FlowSmith/.agent/workspaces/masaakiayb-muselucidsample/.muselucid/plan/ISSUE-0001-requirements.md)

実施した確認:
- `test -f .muselucid/plan/ISSUE-0001-requirements.md` -> `OK`
- `rg` による必須セクション/キーワード確認 -> すべてヒット
- `git diff --check` -> `DIFF_CHECK_OK`

実行ログ記録:
- [coder_output_attempt_1.md](/home/runner/work/FlowSmith/FlowSmith/.agent/runs/masaakiayb-muselucidsample/20260224T121826Z-issue-5/coder_output_attempt_1.md)