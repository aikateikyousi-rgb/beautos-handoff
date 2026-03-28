# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-28 13:03

## HANDOFF_ID
20260328-130326

---

## 稼働サービス
```
  913	0	com.beautos.tunnel
  922	0	com.beautos.ollama
  1229	1	com.beautos.bot
  908	0	com.beautos.watcher
  923	0	com.beautosbrain.personawatcher
  935	0	com.beautos.web
  911	0	com.beautos.evidence-watcher
  933	0	com.beautos.partner
  （停止中 26件）
```

## DB統計
- products.db: 5151件
- ingredients_master.db: 244件

## 直近エラー（各ログ末尾50行）
```
  [pipeline_20260327.log] 2026-03-27 07:00:49,896 ERROR LINE API error: 429 {"message":"You have reached your monthly limit."}
  [pipeline_20260328.log] 2026-03-28 07:00:22,572 ERROR LINE API error: 400 {"message":"Failed to send messages"}
  [pipeline_20260328.log] 2026-03-28 07:00:22,574 ERROR LINE 通知送信失敗
  [pipeline_20260328.log] 2026-03-28 07:00:22,703 ERROR plain text send error: 400 Client Error: Bad Request for url: https://api.line.me/v2/bot/message/push
  [pipeline_20260328.log] 2026-03-28 07:00:55,678 ERROR LINE API error: 400 {"message":"Failed to send messages"}
  [pipeline_20260328.log] 2026-03-28 07:00:55,680 ERROR LINE 通知送信失敗
  [pipeline_20260328.log] 2026-03-28 07:00:55,801 ERROR plain text send error: 400 Client Error: Bad Request for url: https://api.line.me/v2/bot/message/push
  [slack_bot.log] 2026-03-14 23:57:07,644 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SYS] unknown error (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:17,721 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
  [slack_bot.log] 2026-03-14 23:57:27,796 ERROR slack_bolt.App: Failed to check the state of sock (session id: 7d505a4e-beac-4036-8609-3c65397307ec, error: SSLError, message: [SSL: BAD_LENGTH] bad length (_ssl.c:2427))
```

## 直近の変更・handoff内容
```
# BEAUTOS引き継ぎ 2026-03-28

## 本日完了
- handoff基盤の修正（handoff_draft.txt経由でコンテンツが確実に渡るよう修正）
- .zshrcのhandoff関数を優先順位付きで再設計・動作確認済み
- Layer1（Google Docs）・Layer2（GitHub）両方への書き込み確認済み

## 積み残しタスク（優先順・番号付き）
①viewerブランド別確認→Geminiバッチ（商品数多い順）
②全商品バッチ生成（1日500枚×10日）
③beautos_certified
④Instagram
⑤partner LP
⑥CONNECT tier
⑦LINE試験（10名美容師）
⑧Stripe（継続課金チェック→続行から）
⑨法務（ディーラーキックバック）
⑩ImportanceCalibrator（feedback_db 30件到達後）

## システム状態変更
- handoff関数：pbpaste依存 → handoff_draft.txt優先に変更
- ingredients_master.db: 44件→244件（前回比増加を確認）

## 次回やること
viewerブランド別確認から再開
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
