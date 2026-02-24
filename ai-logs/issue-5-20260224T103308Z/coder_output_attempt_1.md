Issue #5 向けに要件仕様を最小差分で更新し、品質ゲートも通過しています。

変更内容:
- [`.muselucid/plan/specs/ISSUE-0001-requirements.md`](/home/runner/work/FlowSmith/FlowSmith/.agent/workspaces/masaakiayb-muselucidsample/.muselucid/plan/specs/ISSUE-0001-requirements.md)
  - `C-01〜C-03` に「合格条件」を追加し、制約を検証可能な表現に統一
  - 検証章に「曖昧語チェック」と「ACのYes/No判定可能性チェック」を追加

実行確認:
- `test -f ...` OK
- `rg -n "^## "` で必須章を確認
- `rg -n "^### FR-0[1-5]"` で FR-01〜FR-05 を確認
- Issueキーワード反映チェック（受注番号/顧客コード/重複/受付ID/処理時刻/10秒/タイムアウト/ステータス別件数）実施済み
- 制約反映チェック（マスキング/DBスキーマ/2か月）実施済み
- `git diff --check` 通過

指定ログ出力:
- [`coder_output_attempt_1.md`](/home/runner/work/FlowSmith/FlowSmith/.agent/runs/masaakiayb-muselucidsample/20260224T103308Z-issue-5/coder_output_attempt_1.md) に実行ログと変更要約を記載済み。