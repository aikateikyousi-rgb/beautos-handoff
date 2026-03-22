# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-22 23:20

## HANDOFF_ID
20260322-232041

---

## 稼働サービス
```
  989	0	com.beautos.tunnel
  997	0	com.beautos.ollama
  1003	0	com.beautos.bot
  984	0	com.beautos.watcher
  998	0	com.beautosbrain.personawatcher
  1008	0	com.beautos.web
  987	0	com.beautos.evidence-watcher
  （停止中 24件）
```

## DB統計
- products.db: 5151件
- ingredients_master.db: 244件

## 直近エラー（各ログ末尾50行）
```
  [pipeline_20260320.log] 2026-03-20 10:51:09,068 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [pipeline_20260320.log] 2026-03-20 10:51:09,070 ERROR LINE 通知送信失敗
  [pipeline_20260320.log] 2026-03-20 10:51:09,174 ERROR plain text send error: 429 Client Error: Too Many Requests for url: https://api.line.me/v2/bot/message/push
  [pipeline_20260321.log] 2026-03-21 23:58:37,110 ERROR [draft_generator] Ollama エラー: timed out
  [pipeline_20260321.log] 2026-03-21 23:58:37,111 ERROR [main] generate_draft エラー: timed out
  [pipeline_20260322.log] 2026-03-22 07:00:22,493 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [pipeline_20260322.log] 2026-03-22 07:00:55,031 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [slack_bot.log] 2026-03-14 23:57:07,644 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SYS] unknown error (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:17,721 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:27,796 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
