要件仕様への落とし込みを実施しました。重複記述を整理し、実装可能なI/O仕様まで明文化しています。

**変更ファイル**
- [`ISSUE-0001.yaml`](/home/runner/work/FlowSmith/FlowSmith/.agent/workspaces/masaakiayb-muselucidsample/.muselucid/plan/issues/ISSUE-0001.yaml)
- [`ISSUE-0001.md`](/home/runner/work/FlowSmith/FlowSmith/.agent/workspaces/masaakiayb-muselucidsample/.muselucid/plan/requirements/ISSUE-0001.md)
- 実行ログ: [`coder_output_attempt_1.md`](/home/runner/work/FlowSmith/FlowSmith/.agent/runs/masaakiayb-muselucidsample/20260224T111226Z-issue-5/coder_output_attempt_1.md)

**対応内容**
- `ISSUE-0001.yaml` の `summary`/`scope` の重複文を正規化。
- 要件仕様書参照 (`.muselucid/plan/requirements/ISSUE-0001.md`) を `scope` に追加。
- `acceptance_criteria` と `verify` を、FR-001〜FR-004対応が確認できる内容に具体化。
- 新規仕様書で以下を定義:
  - 対象ユーザー、現状課題、目標状態、業務フロー
  - 正常系/異常系要件
  - FR-001〜FR-004 の「条件・挙動・出力」表
  - 非機能要件（10秒タイムアウト閾値、判定主体、再実行導線）
  - 受け入れ基準、未決事項（なし）

**検証結果**
- `test -f .muselucid/plan/requirements/ISSUE-0001.md` : OK
- 必須章 `rg` チェック: OK
- 主要要件キーワード網羅 `rg` チェック: OK
- `ISSUE-0001.yaml` の `acceptance_criteria|verify|depends_on|risk` 存在確認: OK
- 曖昧語チェック (`適宜|必要に応じて|可能なら|できれば|など`): 0件
- `git diff --check`: 問題なし