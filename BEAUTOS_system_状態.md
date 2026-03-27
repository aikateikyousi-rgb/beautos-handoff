# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-27 16:28

## HANDOFF_ID
20260327-162823

---

## 稼働サービス
```
  1126	0	com.beautos.tunnel
  1134	0	com.beautos.ollama
  14274	-9	com.beautos.bot
  1122	0	com.beautos.watcher
  1135	0	com.beautosbrain.personawatcher
  1145	0	com.beautos.web
  1124	0	com.beautos.evidence-watcher
  1144	0	com.beautos.partner
  （停止中 25件）
```

## DB統計
- products.db: 5151件
- ingredients_master.db: 244件

## 直近エラー（各ログ末尾50行）
```
  [slack_bot.log] 2026-03-14 23:57:17,721 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:27,796 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [web_error.log] [2026-03-23 23:39:36 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:37 +0900] [26110] [ERROR] Connection in use: ('0.0.0.0', 5004)
  [web_error.log] [2026-03-23 23:39:37 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:38 +0900] [26110] [ERROR] Connection in use: ('0.0.0.0', 5004)
  [web_error.log] [2026-03-23 23:39:38 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:39 +0900] [26110] [ERROR] Connection in use: ('0.0.0.0', 5004)
  [web_error.log] [2026-03-23 23:39:39 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:40 +0900] [26110] [ERROR] Can't connect to ('0.0.0.0', 5004)
```

## 直近の変更・handoff内容
```
テスト
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
