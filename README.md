# Zenn + Claude ブログテンプレート

Claude Code を使って Zenn の記事を管理するためのテンプレートリポジトリです。

## 特徴

- **Claude Code 統合**: スラッシュコマンドで記事作成・レビューが可能
- **記事テンプレート**: 技術記事、チュートリアルなどのテンプレート
- **執筆ガイド**: 記事執筆のベストプラクティス
- **公開ワークフロー**: Zenn への公開手順

## セットアップ

### 1. このテンプレートから新しいリポジトリを作成

GitHub で "Use this template" ボタンをクリックして新しいリポジトリを作成します。

### 2. リポジトリをクローン

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO
```

### 3. 依存関係をインストール

```bash
npm install
```

### 4. Zenn CLI をセットアップ

```bash
npx zenn init
```

### 5. ローカルでプレビュー

```bash
npx zenn preview
```

http://localhost:8000 でプレビューが表示されます。

## 使い方

### 新しい記事を作成

Claude Code で以下のスラッシュコマンドを使用：

```
/new-article
```

または手動で：

```bash
npx zenn new:article
```

### 記事をレビュー

```
/review-article
```

### トピックを探す

```
/find-topics
```

## ディレクトリ構成

```
.
├── .claude/              # Claude Code 設定
│   ├── commands/        # スラッシュコマンド
│   ├── CLAUDE.md        # Claude 設定
│   ├── WRITING_GUIDE.md # 執筆ガイド
│   └── PUBLISHING_WORKFLOW.md # 公開ワークフロー
├── articles/            # Zenn 記事
├── books/               # Zenn 本
├── templates/           # 記事テンプレート
└── package.json         # npm 設定
```

## Zenn との連携

### GitHub リポジトリと連携

1. https://zenn.dev/dashboard/deploys にアクセス
2. リポジトリを選択して連携
3. `published: true` にして push すると自動公開

### 下書きを共有

1. `published: false` のまま push
2. Zenn ダッシュボードからプレビュー URL を取得
3. URL を共有してレビュー依頼

## ライセンス

MIT
