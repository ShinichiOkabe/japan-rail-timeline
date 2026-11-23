# 日本の鉄道　変遷年表２０２６年版（初版） / Japan Railway Timeline — 2026 Edition

1950年以降の日本全国の鉄道路線・駅の開業・延伸・廃止（予定を含む）を、地図と年表で確認できるウェブページです。
日本語と英語に対応しています（画面右上で切り替え、または URL の末尾に `#en` / `#ja`）。

A web page showing how Japan's railway network and stations changed since 1950 (including plans), on a map and a timeline. Japanese and English (switch at the top right, or add `#en` / `#ja` to the URL).

## ファイル / Files

| ファイル | 内容 |
|---|---|
| `index.html` | ページ本体（年表データを含む） |
| `net.json` | 路線網（線路の形と、各区間が存在した年） |
| `stations.json` | 駅 約21,000件（駅名・路線・事業者・営業年・位置） |
| `readings.json` | 駅名の読み（ふりがな）。英語表示のローマ字はここから作ります |

## GitHub Pages で公開する手順 / Publishing on GitHub Pages

1. GitHub で新しいリポジトリを作る（例：`japan-rail-timeline`、Public）。
2. このフォルダの中身（`index.html`、3つの `.json`、`.nojekyll`、`README.md`）をすべてアップロードする（「Add file」→「Upload files」）。
3. リポジトリの「Settings」→「Pages」で、Source を「Deploy from a branch」、Branch を `main` / `(root)` にして「Save」。
4. 数分後、`https://<ユーザー名>.github.io/japan-rail-timeline/` で公開されます。

※ `index.html` をパソコンで直接ダブルクリックして開くと、ブラウザの制限で `.json` を読み込めず路線網が表示されません。GitHub Pages など、ウェブサーバー経由で開いてください。

## 設定 / Settings（`index.html` 内）

- `PAYPAL_URL`：支援ボタンのリンク（現在 `https://paypal.me/marathonBGM`）
- `MAIL`：読みの訂正を受け付けるメールアドレス（現在 `marathonbgm@mbr.nifty.com`）

## 出典 / Sources

- 国土交通省「国土数値情報（鉄道時系列データ）」N05（2025年版）を加工して作成
  （出典：国土交通省国土数値情報ダウンロードサイト https://nlftp.mlit.go.jp/ksj/ ）
- 海岸線：mledoze/countries（ODbL）
- 年表（約500件）の日付は各種公開資料による。予定は2026年11月時点の公表情報
- 駅名の読み（ふりがな）は作成者が付けたもので、誤りを含む可能性があります。お気づきの点はメールでお知らせください。
