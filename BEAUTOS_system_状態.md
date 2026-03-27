# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-27 23:51

## HANDOFF_ID
20260327-235158

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
お疲れ様でした、殿。今日は大きな進展でした。

新チャットにこれをそのまま貼ってください。

---

## 引き継ぎ情報（新チャットに貼ること）

**完了済み**
- フェーズ1：post URL 1071件収集 → `/tmp/mori_post_urls.txt`
- フェーズ2：1071件全文取得 → `/tmp/mori_phase2.jsonl`（1,293,159文字）
- 用語辞書確定 → `/tmp/nagata_glossary.json`（40件）

**次の作業：Ollama構造化パイプライン実装**

構造化スキーマ：
```
statement / category / conditions / failure_mode / evidence_quote / stance
```

カテゴリ固定リスト：
```
ビビリ毛/過還元/過膨潤/熱変性/酸化エラー/酸化不足/過酸化/
薬剤選定/アイロン操作/放置時間/毛髪診断/髪質判定/禁忌/
施術プロセス/酸熱トリートメント/カラー施術/スピエラ/システアミン/チオ/GMT/other
```

設計方針（4AI議会確定版）：
- Ollama（qwen2.5:14b）× Pydantic Schema × temperature=0.0
- Extractor（初回）+ Fixer（修正専用）の2プロンプト分離
- risk_score≥4のみClaude APIにエスカレーション
- nagata_glossary.jsonをプロンプトに注入
- 出力：`/tmp/kb_inbox.jsonl`

**環境**
- Mac Mini（Apple Silicon 32GB）
- Ollama qwen2.5:14b インストール済み
- Python3.14・Playwright環境あり

---

では新チャットで会いましょう、殿！
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
