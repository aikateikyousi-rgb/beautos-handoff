# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-21 07:58

## HANDOFF_ID
20260321-075805

---

## 稼働サービス
```
  1760	0	com.beautos.tunnel
  1769	0	com.beautos.ollama
  2687	0	com.beautos.bot
  1756	0	com.beautos.watcher
  1770	0	com.beautosbrain.personawatcher
  1779	0	com.beautos.web
  1758	0	com.beautos.evidence-watcher
  （停止中 23件）
```

## DB統計
- products.db: 5151件
- ingredients_master.db: 44件

## 直近エラー（各ログ末尾50行）
```
  [pipeline_20260320.log] 2026-03-20 07:10:00,443 ERROR plain text send error: 429 Client Error: Too Many Requests for url: https://api.line.me/v2/bot/message/push
  [pipeline_20260320.log] 2026-03-20 07:20:00,683 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [pipeline_20260320.log] 2026-03-20 07:20:00,684 ERROR LINE 通知送信失敗
  [pipeline_20260320.log] 2026-03-20 07:20:00,751 ERROR plain text send error: 429 Client Error: Too Many Requests for url: https://api.line.me/v2/bot/message/push
  [pipeline_20260320.log] 2026-03-20 10:51:09,068 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [pipeline_20260320.log] 2026-03-20 10:51:09,070 ERROR LINE 通知送信失敗
  [pipeline_20260320.log] 2026-03-20 10:51:09,174 ERROR plain text send error: 429 Client Error: Too Many Requests for url: https://api.line.me/v2/bot/message/push
  [slack_bot.log] 2026-03-14 23:57:07,644 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SYS] unknown error (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:17,721 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:27,796 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
