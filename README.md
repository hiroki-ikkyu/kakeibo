# 家計ノート

日々の支出・サブスク・月次予算を管理するPWAアプリ。

## デプロイ手順（GitHub Pages）

### 1. GitHubにリポジトリを作成

1. [github.com/new](https://github.com/new) にアクセス
2. Repository name: `kakeibo`（好きな名前でOK）
3. **Public** を選択
4. 「Create repository」をクリック

### 2. ファイルをアップロード

リポジトリのページで：

1. 「uploading an existing file」のリンクをクリック
2. `kakeibo/` フォルダの中身をすべてドラッグ＆ドロップ：
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
3. 「Commit changes」をクリック

### 3. GitHub Pagesを有効化

1. リポジトリの **Settings** タブ
2. 左メニューの **Pages**
3. Source: **Deploy from a branch**
4. Branch: **main** / フォルダ: **/ (root)**
5. 「Save」

1〜2分で `https://あなたのユーザー名.github.io/kakeibo/` でアクセス可能になります。

### 4. iPhoneのホーム画面に追加

1. Safariで上記URLにアクセス
2. 共有ボタン（□↑）をタップ
3. 「ホーム画面に追加」を選択
4. 名前を確認して「追加」

これでネイティブアプリのように使えます！

## 機能

- 1日3,000円の予算管理（残り・超過がひと目でわかる）
- 今日・今週（月曜起算）・今月の支出サマリー
- ご褒美ストック（節約分の累計）
- スワイプで削除
- サブスク管理（クレジットカード別）
- 週次/月次レビュー（棒グラフ付き）
- カテゴリの自由追加
- 妻の生活費（月ごと変動対応）
- 月50万円の上限管理
- データはlocalStorageに保存（オフライン対応）
- JSONエクスポート

## 技術

- HTML / CSS / JavaScript（フレームワーク不使用）
- PWA（Service Worker + Web App Manifest）
- localStorage
