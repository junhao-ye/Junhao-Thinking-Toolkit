# Junhao-Thinking-Toolkit

[繁體中文](README.md) · [简体中文](README.zh-CN.md) · [English](README.en.md) · **日本語**

まとまりのないメモから検討すべき問いを整理し、概念の理解、仮説の検証、選択肢の比較、行動計画の作成まで支援する Agent Skill です。12 の基本手法に加え、資料整理、仮説の検証、段階的な問題解決、行動計画に絞った 4 つの使い方があります。目的に合わせて主となる手法を一つ選びます。

## クイックスタート

1. リポジトリをダウンロードするか、Git でクローンします。

   ```sh
   git clone https://github.com/junhao-ye/Junhao-Thinking-Toolkit.git
   ```

2. [`skills/junhao-thinking-toolkit`](skills/junhao-thinking-toolkit) フォルダー全体を、エージェントがスキルを読み込むディレクトリにコピーします。Codex のユーザー用スキルには `~/.codex/skills/` を使用できます。
3. 新しい会話で `junhao-thinking-toolkit` を選ぶか名前を指定し、目的、資料、欲しい成果物を伝えます。

> junhao-thinking-toolkit を使って、以下の問い合わせメモをテーマ別に整理してください。繰り返し出てくる問題と元の記録を対応づけ、優先して確認すべき手がかりを挙げてください。日本語で回答してください。

## 目的別の使い方

| やりたいこと | 指定できる手法 |
| --- | --- |
| 考えを整理する、行き詰まりの原因を明確にする | 資料整理、ソクラテス式問答 |
| 概念を理解する、事例から学ぶ、主張を確かめる | 二段階の解説、事例の逆分析、ファクトチェック |
| 案の弱点や別の解き方を探る | 仮説の検証、専門的な視点からの検討、第一原理思考 |
| 選択肢を比べる、不確実性を検証する、日程を組む | 二案・複数案の比較、小さくやり直せる実験、行動計画 |

全手法の一覧、コピーして使える依頼文、インストールの確認方法、よくある質問は[日本語ユーザーガイド](docs/user-guide.ja.md)を参照してください。

## ファイルと出典

手法の選び方と共通の実行ルールは [SKILL.md](skills/junhao-thinking-toolkit/SKILL.md) にあり、各手法の手順は [references/](skills/junhao-thinking-toolkit/references) にまとまっています。

基本手法は數字生命卡茲克（Khazix）の手法をもとにしています。提供された図解の 10 の手法をどこに取り入れたかは、[出典と対応表](skills/junhao-thinking-toolkit/SOURCES.md)に記載しています。
