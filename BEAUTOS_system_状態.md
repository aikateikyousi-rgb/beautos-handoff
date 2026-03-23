# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-23 20:51

## HANDOFF_ID
20260323-205159

---

## 稼働サービス
```
  989	0	com.beautos.tunnel
  997	0	com.beautos.ollama
  21877	0	com.beautos.bot
  984	0	com.beautos.watcher
  998	0	com.beautosbrain.personawatcher
  19985	0	com.beautos.web
  987	0	com.beautos.evidence-watcher
  （停止中 24件）
```

## DB統計
- products.db: 5151件
- ingredients_master.db: 244件

## 直近エラー（各ログ末尾50行）
```
  [pipeline_20260323.log] 2026-03-23 07:00:24,628 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [pipeline_20260323.log] 2026-03-23 07:00:57,878 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [slack_bot.log] 2026-03-14 23:57:07,644 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SYS] unknown error (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:17,721 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:27,796 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [web_error.log] [2026-03-23 19:59:01 +0900] [19985] [ERROR] Worker (pid:19988) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-23 19:59:07 +0900] [19985] [ERROR] Worker (pid:20009) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-23 19:59:18 +0900] [19985] [ERROR] Worker (pid:19987) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-23 19:59:27 +0900] [19985] [ERROR] Worker (pid:20075) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-23 19:59:58 +0900] [19985] [ERROR] Worker (pid:20029) was sent SIGKILL! Perhaps out of memory?
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
