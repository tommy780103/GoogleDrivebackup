# GoogleDrivebackup

## 最初に読む
未読の共通ルールを次の順で読み、この案件のREADME.mdと関連する直近の_docsを確認する。

```text
/Users/tommy/my-workspace/AGENTS.md
/Users/tommy/my-workspace/dev/AGENTS.md
/Users/tommy/my-workspace/dev/infra/AGENTS.md
```

## この案件
- 目的：個人用Google Driveバックアップツールの案内・プライバシーポリシーを公開する。
- 地図：site/index.htmlがホームページ、site/privacy.htmlがプライバシーポリシー。README.mdが運用案内、_docsが実装・検証記録。
- 公開：GitHubのtommy780103/tommy780103.github.ioリポジトリのmain直下へ、site内のHTML2枚だけを配置する。
- 確認：ローカル確認は以下のコマンドで起動し、ブラウザで2ページと相互リンクを確認する。公開後は公開URLのHTTP応答と本文も読み戻す。

```sh
python3 -m http.server 8000 --bind 127.0.0.1 --directory site
```

- 設定・トークン・バックアップファイルは公開しない。この案件全体を公開リポジトリへ一括送信しない。
- 重要な変更と検証結果は_docsに記録する。案件の新設・移動・終了時は開発索引を更新する。
