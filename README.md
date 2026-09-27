# rclone-backup 公開サイト

個人のMacを本人のGoogleドライブへバックアップするツールについて、ホームページとプライバシーポリシーを案内する静的サイトです。

## 構成
- site/index.html：ホームページ。
- site/privacy.html：プライバシーポリシー。
- _docs：実装・検証記録。
- AGENTS.md：この案件の作業案内。

HTMLとページ内CSSのみを使用します。外部スクリプト、外部フォント、解析タグはありません。

## 公開先
リポジトリ：

```text
https://github.com/tommy780103/tommy780103.github.io
```

ホームページ：

```text
https://tommy780103.github.io/
```

プライバシーポリシー：

```text
https://tommy780103.github.io/privacy.html
```

GitHub Pagesはmainブランチのルートを公開元にします。site内のHTML2枚をリポジトリ直下へ配置します。

## ローカル確認
この案件のディレクトリで実行します。

```sh
python3 -m http.server 8000 --bind 127.0.0.1 --directory site
```

ブラウザで開き、2ページの本文・レイアウト・相互リンクを確認します。

```text
http://127.0.0.1:8000/
```

公開後にはHTTPSで両方のURLを開き、HTTP 200と最新本文を確認します。実施結果は_docsへ記録します。

## 公開内容
プライバシーポリシーは個人利用を前提とし、Google Driveへのバックアップ送信を明記します。バックアップ用途との矛盾を避けるため「外部サーバーへの送信は一切しない」という表現は使用しません。

このサイトは案内用です。Google Cloudのブランディング変更、OAuthクライアント作成、実際のバックアップ設定は、このサイトの作成作業には含みません。
