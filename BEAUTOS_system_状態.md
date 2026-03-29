# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-30 00:59

## HANDOFF_ID
20260330-005909

---

## 稼働サービス
```
  913	0	com.beautos.tunnel
  922	0	com.beautos.ollama
  53652	-15	com.beautos.bot
  44664	-9	com.beautos.watcher
  923	0	com.beautosbrain.personawatcher
  44667	-9	com.beautos.web
  44670	-9	com.beautos.evidence-watcher
  44672	-9	com.beautos.partner
  （停止中 18件）
```

## DB統計
- products.db: 5151件
- ingredients_master.db: 244件

## 直近エラー（各ログ末尾50行）
```
  [slack_bot.log] 2026-03-14 23:57:07,644 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SYS] unknown error (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:17,721 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:27,796 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [web_error.log] [2026-03-29 23:44:20 +0900] [44667] [ERROR] Worker (pid:44675) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-29 23:44:24 +0900] [44667] [ERROR] Worker (pid:44674) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-29 23:50:05 +0900] [44667] [ERROR] Worker (pid:52218) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-29 23:55:52 +0900] [44667] [ERROR] Worker (pid:52217) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-30 00:00:32 +0900] [44667] [ERROR] Worker (pid:52381) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-30 00:00:52 +0900] [44667] [ERROR] Worker (pid:52286) was sent SIGKILL! Perhaps out of memory?
  [web_error.log] [2026-03-30 00:02:57 +0900] [44667] [ERROR] Worker (pid:52970) was sent SIGKILL! Perhaps out of memory?
```

## 直近の変更・handoff内容
```
# BEAUTOS引き継ぎ 2026-03-30
## 本日完了
- nagata_comment_generator.py 完成・動作確認済み（禁止ワード・口調・開始ルール・成分マッチング全修正）
- hair_knowledge_scraper.py に特約店4ブランド追加（オージュア・サブリミック・WELLA・バイカルテ）
## 積み残しタスク
1. hair_scraper完了確認（PID:53717 バックグラウンド実行中・約5〜6時間）→ 完了後にevidence_finder実行 → nagata_comment本番生成
2. 4/1リニューアル告知配信（642人）← 残り2日
3. リッチメニュー更新
4. ハッシュタグ検知実装
5. beautos_certified カラム追加
6. Instagram @nagata_beautos 開設
7. partner LP / CONNECT tier
## システム状態変更
- hair_scraper バックグラウンド実行中（PID:53717）
- store_brain.db: hair_knowledge 40件以上（増加中）
- nagata_comment_generator.py: 完成済み・本番待機中
## 次回やること
- tail ~/beautos-platform/logs/hair_scraper_20260329.log で完了確認
- evidence_finder実行 → nagata_comment全件生成
- 4/1告知配信文面作成・送信
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
