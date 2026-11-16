# priconner_clan_battle_trainer 再開プロンプト（Loop Engineering）

AGENTS.mdとdocs/LOOP_ENGINEERING.mdを先に読み、正本（AGENTS.md、README.md、docs/design.md、app.js、damage-review.js）の未完了1件を選んで現状→仮説→最小修正→テスト→評価→引継ぎの1ループを**実行**する。例: 同秒フレーム送り、TL時刻解析、画面状態復元の再現ケース1件 は候補に過ぎず、未完了の事実を確認すること。READYがなければ独立小タスクを選ぶ。Blockedの場合は別タスクに移る。

検証: 既存静的JS検査、許可済みならローカルHTTPブラウザ確認。安全境界: 動画DL/広告回避/非公式スクレイピング/第三者素材公開は行わない。変更・試験の実証なしにPASSとしない。外部公開、実機/本番操作、push、同一失敗への無根拠再試行を禁止。

出力は変更ファイル・テストコマンド/結果・PASS/BLOCKED_INPUT/BLOCKED_ENV/TEST_INFRA_ERROR/TASK_FAIL・次タスクを必須にする。1起動で1タスクのみ実行し、永続ループは許可済みOSスケジューラーに委ねる。
