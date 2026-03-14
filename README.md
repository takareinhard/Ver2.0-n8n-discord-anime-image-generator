# n8n Discord Anime Image Generator

Discordで `!anime` コマンドを受け取り、Fal APIでアニメ画像を生成してDiscordへ返す n8n ワークフローです。

## 概要

- Discordの `!anime` をトリガーに実行
- プロンプトに補助文を自動追加
- Fal APIで画像生成
- 成功時は画像URLをDiscordに返信
- 失敗時は `画像生成に失敗しました` とエラー文を返信

## 今回の修正

- `HTTP Request` ノードをエラー継続に変更
- エラー本文を抽出するノードを追加
- Discordへ失敗通知を返す分岐を追加

## 使い方

1. `workflow.sanitized.json` をn8nにインポートします。
2. Discord Bot Trigger / Discord Bot / Fal API の認証を設定します。
3. `YOUR_GUILD_ID` と `YOUR_CHANNEL_ID` を置き換えます。
4. ワークフローを有効化します。

## 注意

- 公開版JSONには認証情報を入れないでください。
- `magicPrompt` は好みの画風に合わせて調整できます。
