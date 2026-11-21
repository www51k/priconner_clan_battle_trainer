# progress.md — priconner_clan_battle_trainer

<!-- progress-collection:v1
{"project_id":"priconner_clan_battle_trainer","monitor":true,"instruction_target":"existing-codex","dispatch_policy":"verified-only","host":null,"thread_id":null,"status":"PAUSED_BY_USER","last_verified_at":null}
-->


## 管理状態（2026-11-22 利用者指定）
- **監視対象のまま保留（PAUSED_BY_USER）**。進捗・状態の確認は可能だが、タスクの起動・再開は禁止。
- 現時点で急ぎの実装作業なし。ユーザーの再開指示まで実装・テストの自動起動や既存Codexへの作業指示を行わない。
- 現地PCのCodex/OSタスクループが停止していることは未検証。ローカル設定の `enabled: false` /停止マーカー/スレッド所有者を確認するまでは停止完了とみなさない。
- 再開は利用者の明示指示と既存担当・停止条件の再照合後のみ。

## 監視・指示対象
- `progress-collection` の監視対象であり、既存担当Codexへの指示候補。現地PC・thread ID未確認で**指示は未送信**。
- `NEEDS_TRIAGE` は未完了確認待ちであってREADY/作業中/PASSではない。ユーザー停止指示、実機・外部送信の承認を優先。

## 正本照合が必要な小タスク候補
- [ ] ブラウザのフレーム移動/目押しログ/ダメージ比較に関する既存の再現可能な1件。YouTube非公式取得禁止。
- 例示は未完了の保証ではない。ソース・実テスト・既存差分を確認して選択し、完了済みなら別の独立案件を探す。

## 作業記録
| 時刻 | task_id | 状態 | 変更ファイル | 検証結果 | ブロッカー | 次の独立タスク |
| --- | --- | --- | --- | --- | --- | --- |
| 未実施 | 未確定 | NEEDS_TRIAGE | なし | 未検証 | 既存担当の確認待ち | 正本に基づく実行可能な小タスク1件 |

## 1サイクル
現状→仮説→最小変更→テスト→分類→次の一手。必ず実コード変更/検証の根拠に基づいてstatusと履歴を更新。監視だけでPASSにしない。
