# ペルセウスの試練 レビュー用テスト版

ChatGPTに初見プレイしてもらうための、テスト専用のコピーです。
本番（Claudeのアーティファクト）とは別のファイルで、本番のファイルやセーブデータには影響しません。

## 本番との違い

- 画面に最短ターン数（神々の記録の数字）を表示しない（「？？」と表示）
- ステージデータから正解手順を取り除いてある
- セーブデータは別の保存名（perseus-review-progress）。本番の記録とは混ざらない
- 検索エンジンに載らないよう指定（noindex）
- ゲームのルール、ステージ、難易度、ヒント機能は本番と同じ

## GitHub Pagesで公開する手順（ブラウザだけでできます）

1. GitHubにログインし、右上の「+」→「New repository」
2. Repository name に `perseus-review` などと入力
3. 公開範囲は「Public」を選ぶ（無料プランのGitHub Pagesは公開リポジトリのみ対応）
4. 「Create repository」
5. 「uploading an existing file」をクリックし、この `index.html` をドラッグして「Commit changes」
6. リポジトリの「Settings」→ 左の「Pages」
7. 「Build and deployment」の Source を「Deploy from a branch」、Branch を「main」「/ (root)」にして「Save」
8. 1〜2分待つと、Pagesの画面上部に公開URL（https://ユーザー名.github.io/perseus-review/）が表示される

## テストが終わったら（公開の停止）

- 一時停止：リポジトリの「Settings」→「Pages」→ 公開URLの横の「…」→「Unpublish site」
- 完全に消す：「Settings」→ 一番下の「Delete this repository」

## 公開中に気をつけること

- URLを知っている人は誰でも遊べます。リポジトリも公開なので、ゲームのコードと絵は誰でも見られます
- ファイルに個人情報、パスワード、APIキーなどは含まれていません（確認済み）
- URLに GitHub のユーザー名が入ります
- 画面の文字フォントを Google Fonts から読み込みます（読み込めなくても、別の文字で遊べます）
