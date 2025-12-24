# 岩盤置換プラグイン

岩盤を平坦化して洞窟を埋めるMinecraftプラグイン

## 概要

洞窟を検出して岩盤（Bedrock）を平坦化するプラグインです。
Y-64以外の岩盤ブロックを、深層岩ブロックに変換します。
大規模な地形整備や、洞窟による問題を解決できます。

## 主な機能

- 洞窟の自動検出と岩盤での埋め立て
- チャンク単位での一括処理
- 処理量制限による安全な実行
- 処理のキャンセル機能
- 詳細な権限設定

## ダウンロード

[Releases](https://github.com/あなたのユーザー名/BedrockReplacer/releases)から最新版をダウンロードしてください。

## インストール方法

1. [Releases](https://github.com/あなたのユーザー名/BedrockReplacer/releases)から`.jar`ファイルをダウンロード
2. サーバーの`plugins`フォルダに配置
3. サーバーを再起動
4. `plugins/BedrockReplacer/config.yml`で設定を調整（任意）

## コマンド

| コマンド | 説明 | 権限 |
|---------|------|------|
| `/bedrockflat <半径>` | プレイヤーの周囲を平坦化 | `bedrockreplacer.flat` |
| `/bedrockchunk <チャンク数>` | チャンク単位で処理 | `bedrockreplacer.chunk` |
| `/bedrockcancel` | 処理をキャンセル | `bedrockreplacer.cancel` |
| `/bedrockreload` | 設定を再読み込み | `bedrockreplacer.reload` |

## パーミッション
```yaml
bedrockreplacer.flat    # /bedrockflat の使用権限
bedrockreplacer.chunk   # /bedrockchunk の使用権限
bedrockreplacer.cancel  # /bedrockcancel の使用権限
bedrockreplacer.reload  # /bedrockreload の使用権限
```

## 設定

`config.yml`:
```yaml
max-volume: 1000000  # 最大処理ブロック数
max-chunks: 100      # 最大処理チャンク数
```

## 動作環境

- Spigot/Paper 1.21.x
- Java 17以上

## 注意事項

- 大規模な処理は負荷がかかるため、プレイヤーが少ない時間帯に実行することを推奨
- 処理前にワールドのバックアップを取ることを推奨

## 実際に使用しているサーバー

このプラグインは250人以上が参加する日本人向けMinecraftサーバーで使用されています。

**Discordサーバー:** https://discord.gg/zYY55dzhjd

サーバーの特徴：
- サバイバルゲームプレイ
- カスタムプラグイン多数
- エコノミーシステム・クイズイベント等
- 活発な開発とアップデート

お気軽にご参加ください！

## サポート

- バグ報告・機能要望: [Issues](https://github.com/あなたのユーザー名/BedrockReplacer/issues)
- 質問・サポート: [Discord](https://discord.gg/zYY55dzhjd)

## ライセンス

All Rights Reserved（個人使用のみ許可、再配布・改変禁止）

---

SpigotMCでも配布中: [BedrockReplacer on SpigotMC](https://www.spigotmc.org/resources/あなたのリソースID/)
