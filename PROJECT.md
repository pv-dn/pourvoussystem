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

**共有コードなし。** 以下とは完全に別プロジェクト・別フォルダ・別ワークスペース。

- **価格参照**（`Apps\価格参照`）— 客先別単価の参照専用。品番・単価は JSON / Firestore から**読み取り連携**するが、アプリ・コード・セッションは別
- プゥルヴー在庫（`Apps\プゥルヴー在庫`）— 在庫管理
- ライフ伝票（`Apps\ライフ伝票`）— 別会社伝票

## Cursor で開くとき

- `Apps\Cursor用\workspaces\プゥルヴー伝票.code-workspace` を使う（価格参照フォルダは足さない）

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
| 2026-07-13 | 運用方法を折りたたみ式に更新（未発行・売上統計・Firebase同期など現状に合わせて刷新） |
| 2026-07-11 | 未発行お知らせは左サイドバーのみに再統一（中央ポップアップ・バナー・ベルを削除） |
| 2026-07-11 | 未発行お知らせカード（ログイン時ポップアップ・ヘッダーベル・上部バナー）を復元 |
| 2026-07-01 | 未発行お知らせを目立つように改善（バナー・点滅ボタン・ログイン時モーダル） |
| 2026-07-01 | `Apps\プゥルヴー伝票` に正本フォルダ・ワークスペースを整備 |
