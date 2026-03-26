# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-26 19:42

## HANDOFF_ID
20260326-194209

---

## 稼働サービス
```
  70472	0	com.beautos.tunnel
  997	0	com.beautos.ollama
  76716	-15	com.beautos.bot
  984	0	com.beautos.watcher
  998	0	com.beautosbrain.personawatcher
  44623	0	com.beautos.web
  987	0	com.beautos.evidence-watcher
  71691	-15	com.beautos.partner
  （停止中 21件）
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

## 直近の変更・handoff内容
```
Last login: Thu Mar 26 18:43:21 on ttys006
gonagata@gonoMac-mini ~ % mkdir -p ~/AI_Adult/{Models,Generated,Scripts,Prompts,Logs}
gonagata@gonoMac-mini ~ % mdutil -i off ~/AI_Adult
/System/Volumes/Data/Users/gonagata/AI_Adult:
Error: invalid operation.
	Error: unknown indexing state.
gonagata@gonoMac-mini ~ % >....
gonagata@gonoMac-mini ~ % mkdir -p ~/AI_Adult/{Models,Generated,Scripts,Prompts,Logs}
gonagata@gonoMac-mini ~ % mdutil -i off ~/AI_Adult
/System/Volumes/Data/Users/gonagata/AI_Adult:
Error: invalid operation.
        Error: unknown indexing state.
gonagata@gonoMac-mini ~ % Last login: Thu Mar 26 18:43:21 on ttys006
gonagata@gonoMac-mini ~ % mkdir -p ~/AI_Adult/{Models,Generated,Scripts,Prompts,Logs}
gonagata@gonoMac-mini ~ % mdutil -i off ~/AI_Adult
/System/Volumes/Data/Users/gonagata/AI_Adult:
Error: invalid operation.
        Error: unknown indexing state.
gonagata@gonoMac-mini ~ %
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
