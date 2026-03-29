# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-30 00:53

## HANDOFF_ID
20260330-005354

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
- GitHub二層目廃止・handoff一層化確定
- image-fetcher/image-scraper停止・削除（Hyumi12件lifekarte URL復元済み）
- 不要バッチ8本削除（meo/connect/interview/brain.growth/brand-scraper/category-classifier/stockmonitor）
- neta_hunter→seed_knowledge パイプライン修通（pending直投入）
- BEAUTOS管理通知LINE（@020ymzto）送信切り替え完了（毎朝7時Flexカード）
- Telegramフォールバック廃止
- ADMIN_LINE_ID更新（Uc043e9eabc27cae9e6a7b55f10d77aef）

## 積み残しタスク（優先順）
① 特約店4ブランド公式URL→hair_scraper→evidence_scores補強→nagata_comment本番生成
② 履歴を覚える機能（chat_history蓄積）
③ ハッシュタグ検知実装
④ 4/1リニューアル告知配信（642人）
⑤ リニューアル3点セット（アカウント名変更・リッチメニュー更新・AI相談稼働告知）
⑥ beautos_certifiedカラム追加
⑦ Instagram @nagata_beautos 開設
⑧ partner LP / CONNECT tier設計

## システム状態変更
- ADMIN_LINE_ID=Uc043e9eabc27cae9e6a7b55f10d77aef
- line_notifier送信先：@020ymzto（管理通知）に変更
- LINE_NOTIFY_ACCESS_TOKEN：@020ymztoのトークンに更新
- webhook/notify エンドポイント追加（bot.beautos-ai.com/webhook/notify）
- neta_candidates.json：pending→RAG直投入に変更
- 不要バッチ8本のplist削除済み

## 次回やること
nagata_comment本番生成（store_brain.db充実が先決）
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
