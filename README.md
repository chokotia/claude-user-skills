# Claude User Skills

自分の全ての開発プロジェクトで共通して利用する、Claude Code 用の自作スキル（Agent Skills）を管理するリポジトリです。

## 収録スキル

### 1. commit
- **概要**: `git diff --staged` を元に、プロジェクト規約に沿ったコミットメッセージを生成・実行します。
- **特徴**: ステージングと最終確認を人間が行う、安全なフローを採用しています。

## 導入方法

このリポジトリを任意の場所にクローンします（例: `~/src/claude-user-skills`）。

### 各プロジェクトへの適用

各プロジェクトのルートディレクトリで、以下のコマンドを実行してシンボリックリンクを作成します。

#### Windows (PowerShell)
```powershell
mkdir .claude
cmd /c mklink /J .claude\skills C:\path\to\claude-user-skills\skills
```

#### Linux / Mac
```bash
mkdir -p .claude
ln -s ~/path/to/claude-user-skills/skills .claude/skills
```
