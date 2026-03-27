# BEAUTOS システム状態（handoff自動生成）

## 更新日時
2026-03-28 08:12

## HANDOFF_ID
20260328-081219

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
了解です。では今夜03:00のlaunchdから新プロンプトで回ります。

本日はここまでで十分な進捗です。セッション終了プロトコルに入りましょう。

**「DONE!をタイトルに入れて」**をお忘れなく、殿。

引き継ぎ文を生成します：

```
# BEAUTOS引き継ぎ 2026-03-28

## 本日完了
- ミルボン（151001）313件を生成対象に追加
- チューリップ→5シーン新プロンプトに刷新（大理石・窓辺・バスルーム・ドレッサー・キャンドル）
- uprightを強化（grounded・bottom touching surface）
- dressing table→white marble vanity surfaceに変更
- 特約店旧s01（427枚）削除→再生成キュー入り
- launchd毎晩03:00自動実行登録（com.beautos.generate_tokuyakuten）
- 初日490枚完了（エラーゼロ）
- SHOPギャラリー5枚スワイプ表示実装
- brand_name_enカラムDB追加（Aujua/Wella/Sublimic/Milbon/Bykarte）
- SEO keywords metaにbrand_name_en追加

## 積み残しタスク（優先順・番号付き）
①画像生成継続（毎晩03:00自動・約7日で全完了）
②残り全商品（その他ブランド）画像生成→バイカルテ以降
③beautos_certified
④Instagram
⑤partner LP
⑥CONNECT tier
⑦LINE試験（10名美容師）
⑧Stripe（LINE友だち増加後・継続課金チェック→続行から）
⑨法務（ディーラーキックバック）
⑩ImportanceCalibrator（feedback_db 30件到達後）
⑪Note PRO
⑫ケモカール記事
⑬nagata_comment全件生成
⑭KOUMEI_RULES登録

## システム状態変更
- products.db: brand_name_enカラム追加済み
- generate_tokuyakuten.py: 5シーン対応・upright強化・大理石統一
- generate_images.py: 同上
- launchd: com.beautos.generate_tokuyakuten（毎日03:00）登録済み
- shop_routes.py: ギャラリー5枚スワイプ・SEO keywords追加済み

## 次回やること
- 画像生成進捗確認（ls ~/beautos-platform/data/images/generated/ | wc -l）
- 生成済み画像をSHOPで目視確認
- 次フェーズ：その他ブランド全件画像生成
```
```

---

## 既知の未解決問題
```
（handoff 実行時に手動で記入してください）
```
