要件仕様書を Issue #5 のスコープで新規作成し、曖昧表現を解消しました。

変更ファイル:
- [ISSUE-0001-requirements.md](/home/runner/work/FlowSmith/FlowSmith/.agent/workspaces/masaakiayb-muselucidsample/.muselucid/plan/ISSUE-0001-requirements.md)
- [coder_output_attempt_1.md](/home/runner/work/FlowSmith/FlowSmith/.agent/runs/masaakiayb-muselucidsample/20260224T115942Z-issue-5/coder_output_attempt_1.md)

実施内容:
- As-Is/課題/目的/スコープを分離し、重複記述を整理。
- FR-01〜FR-04 を「入力・判定条件・システム動作・ユーザー表示」で実装可能粒度に明文化。
- バリデーション順序を固定（必須チェック→重複チェック→登録→タイムアウト判定）。
- 10秒タイムアウト制約、受け入れ条件、検証観点、未決事項を追加。
- `すぐに` を削除し、測定可能な表現に統一。

検証結果:
- `test -f .muselucid/plan/ISSUE-0001-requirements.md` : OK
- 必須7セクション検索: すべてヒット
- 必須機能要件キーワード検索: 4要件分を確認
- 曖昧語検索（`適宜|必要に応じて|できるだけ|すぐに`）: ヒットなし
- `git diff --check`: 問題なし