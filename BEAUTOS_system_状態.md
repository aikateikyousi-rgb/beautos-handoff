# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-19 22:43

## HANDOFF_ID
20260319-224324

---

## 稼働サービス
```
  945	0	com.beautos.tunnel
  4272	0	com.beautos.ollama
  39076	-9	com.beautos.bot
  64813	0	com.beautos.watcher
  956	0	com.beautosbrain.personawatcher
  35566	0	com.beautos.web
  （停止中 21件）
```

## DB統計
- products.db: 5151件
- ingredients_master.db: 44件

## 直近エラー（各ログ末尾50行）
```
  [pipeline_20260319.log] 2026-03-19 07:00:05,172 ERROR plain text send error: 429 Client Error: Too Many Requests for url: https://api.line.me/v2/bot/message/push
  [pipeline_20260319.log] 2026-03-19 07:10:00,724 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [pipeline_20260319.log] 2026-03-19 07:10:00,725 ERROR LINE 通知送信失敗
  [pipeline_20260319.log] 2026-03-19 07:10:00,800 ERROR plain text send error: 429 Client Error: Too Many Requests for url: https://api.line.me/v2/bot/message/push
  [pipeline_20260319.log] 2026-03-19 07:20:01,196 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [pipeline_20260319.log] 2026-03-19 07:20:01,197 ERROR LINE 通知送信失敗
  [pipeline_20260319.log] 2026-03-19 07:20:01,262 ERROR plain text send error: 429 Client Error: Too Many Requests for url: https://api.line.me/v2/bot/message/push
  [slack_bot.log] 2026-03-14 23:57:07,644 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SYS] unknown error (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:17,721 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:27,796 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
```

## 直近の変更・handoff内容
```
# 進化する脳システムの監視機能設計

**Created:** 3/18/2026 1:23:12  
**Updated:** 3/18/2026 1:48:33  
**Exported:** 3/19/2026 22:43:22  
**Link:** [https://claude.ai/chat/ffa750e5-912f-4467-b022-462e1693c8c7](https://claude.ai/chat/ffa750e5-912f-4467-b022-462e1693c8c7)  



---
Powered by [Claude Exporter](https://www.ai-chat-exporter.net)
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
