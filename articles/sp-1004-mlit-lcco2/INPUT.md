# 話題（選別パイプラインの出力）

- 題（見出し要約）: 国交省、建築物の生涯CO2排出を評価する2028年度の新制度の具体化に着手
- 原題: 建築物の生涯CO2排出を評価へ、国交省が2028年度新制度の具体化に着手
- Springl のカテゴリ（選別時）: カーボンニュートラル
- 選別時の検証: D（PR・転載のみ。独立媒体 0、全 1 媒体）／ 一次情報: 未取得
- 執筆マニュアル: `takkamano/springl-news` の `writing/MANUAL.md`（v2.2）

## 報道（一次情報を探す手がかり。記事の根拠にはしない）
- liv-plus.jp「建築物の生涯CO2排出を評価へ、国交省が2028年度新制度の具体化に着手」2026-10-03 https://liv-plus.jp/business_news/54638/

## 状況（2026-10-04、クラウドのセッション）
執筆は止めている。理由は2つ。

1. **一次情報を取得できない。** このセッションのネットワーク制限で、次のホストに接続できない（403）。
   `www.mlit.go.jp`、`liv-plus.jp`、`news.yahoo.co.jp`、`www.shutterstock.com` ほか。
   使えたのは検索だけで、検索の要約は資料どうしで食い違いがあった（閣議決定の年、第三者認証の有無など）。
   P番号つきの原文（`src/`）が作れないので、事実表・機械点検・監修（MANUAL §1 ②〜⑧）を通せない。
2. **10月の新しい発表を特定できない。** 検索で確認できた国交省の動きは、改正建築物省エネ法の成立（2026年7月）、
   「建築物のライフサイクルカーボンの算定・評価等を促進する制度に関する検討会」（2025年6月〜）まで。
   liv-plus の「具体化に着手」の根拠になった10月の発表は見つからなかった。
   根拠が7月の法改正なら、MANUAL §1 ②の「公開から1か月を超えているとき」にあたる。

## 一次情報の候補（検索で見つけた URL。未取得）
- 報道発表「建築物のエネルギー消費性能の向上等に関する法律の一部を改正する法律案」を閣議決定 https://www.mlit.go.jp/report/press/house05_hh_001129.html
- 検討会のページ https://www.mlit.go.jp/jutakukentiku/build/jutakukentiku_house_tk4_000302.html
- 第1回検討会の報道発表 https://www.mlit.go.jp/report/press/house04_hh_001276.html
- 第四次答申（建築物のライフサイクルカーボン評価の促進） https://www.mlit.go.jp/report/press/content/001978670.pdf
- 報道発表の資料（中身は未確認） https://www.mlit.go.jp/report/press/content/001991074.pdf ／ https://www.mlit.go.jp/report/press/content/001991075.pdf
- 審議会の資料（中身は未確認） https://www.mlit.go.jp/policy/shingikai/content/001997745.pdf

## 再開するときにすること
1. `mlit.go.jp` と `liv-plus.jp` に接続できる環境で、liv-plus の記事から根拠になった国交省の発表を特定する。
2. その発表の公開日を確かめる（1か月を超えていれば、書く前に天野さんに確認する）。
3. MANUAL §1 の②から先へ進む（`fetch_src.py` → `facts1.json` → `draft1.txt` → `check.py` → 監修 → `websearch_check.py` → `wp1.json`）。
