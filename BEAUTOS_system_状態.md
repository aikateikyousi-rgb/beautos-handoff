# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-23 23:42

## HANDOFF_ID
20260323-234200

---

## 稼働サービス
```
  989	0	com.beautos.tunnel
  997	0	com.beautos.ollama
  24616	-15	com.beautos.bot
  984	0	com.beautos.watcher
  998	0	com.beautosbrain.personawatcher
  26107	0	com.beautos.web
  987	0	com.beautos.evidence-watcher
  （停止中 23件）
```

## DB統計
- products.db: 5151件
- ingredients_master.db: 244件

## 直近エラー（各ログ末尾50行）
```
  [web_error.log] [2026-03-23 23:39:35 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:36 +0900] [26110] [ERROR] Connection in use: ('0.0.0.0', 5004)
  [web_error.log] [2026-03-23 23:39:36 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:37 +0900] [26110] [ERROR] Connection in use: ('0.0.0.0', 5004)
  [web_error.log] [2026-03-23 23:39:37 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:38 +0900] [26110] [ERROR] Connection in use: ('0.0.0.0', 5004)
  [web_error.log] [2026-03-23 23:39:38 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:39 +0900] [26110] [ERROR] Connection in use: ('0.0.0.0', 5004)
  [web_error.log] [2026-03-23 23:39:39 +0900] [26110] [ERROR] connection to ('0.0.0.0', 5004) failed: [Errno 48] Address already in use
  [web_error.log] [2026-03-23 23:39:40 +0900] [26110] [ERROR] Can't connect to ('0.0.0.0', 5004)
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
