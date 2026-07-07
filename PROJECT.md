# プゥルヴー伝票（pourvoussystem）

| 項目 | 内容 |
|------|------|
| **ID** | `pourvoussystem` |
| **呼び名** | プゥルヴー伝票 |
| **フォルダ** | `C:\Users\e--yo\Apps\プゥルヴー伝票` |
| **会社** | 株式会社プゥル・ヴー（ホワイト事業部） |

## 概要

納品書・伝票の発行・履歴・客先単価管理。単体 HTML が正本。Firebase で複数 PC 同期。

## 技術スタック

- 単体 HTML（`index.html` が正本）
- Firebase Auth + Firestore（プロジェクト `pourvoussystem`）
- SheetJS（Excel 入出力）
- GitHub Pages デプロイ

## 主要ファイル

| パス | 内容 |
|------|------|
| `index.html` | **正本**（編集はここだけ） |

## 本番 URL

https://pv-dn.github.io/pourvoussystem/

## リポジトリ

https://github.com/pv-dn/pourvoussystem

## 他アプリとの関係

**共有コードなし。** 以下とは完全に別プロジェクト・別データ。

- プゥルヴー在庫（`Apps\プゥルヴー在庫`）— 在庫管理
- ライフ伝票（`Apps\ライフ伝票`）— 別会社伝票

## デプロイ

```powershell
cd "C:\Users\e--yo\Apps\プゥルヴー伝票"
git add index.html
git commit -m "変更内容の説明"
git push origin main
```

## 変更履歴メモ

| 日付 | 内容 |
|------|------|
| 2026-07-01 | 未発行お知らせを目立つように改善（バナー・点滅ボタン・ログイン時モーダル） |
| 2026-07-01 | `Apps\プゥルヴー伝票` に正本フォルダ・ワークスペースを整備 |
