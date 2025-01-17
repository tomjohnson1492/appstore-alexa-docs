---
title: リリースノート
permalink: fire-app-builder-release-notes.html
sidebar: fireappbuilder_ja
product: Fire App Builder
toc: false
github: true
---

## バージョン 1.0.0

### 機能

Fire App Builderの最初のリリースが 2016 年 10 月 1 日にGithubに公開されました。最初のリリースには、メディアフィードの解析とメディアの再生が可能なJavaベースのAndroid TVアプリが機能制限なしで含まれています。

また、10 種類以上のコンポーネントが用意されており、開発者は分析、広告、アプリ内課金機能、およびメディアプレーヤーのコンポーネントをアプリに簡単に追加できます。XMLファイルやJSONファイルに値を設定すれば、フォント、画像、色、レイアウトなど、アプリのルックアンドフィールをカスタマイズできます。


### 既知の問題・よくあるトラブル {#known_issues}

*  *Facebook認証コンポーネント。* [Facebook認証コンポーネント][fire-app-builder-facebook-auth-component]を使用している場合、このコンポーネントによってメッセージが表示されたときにユーザーが [Log in Later] を選択しても、それ以降にログインするよう求められることがありません(本来は、一定時間が経つとメッセージが再度表示される必要があります)。
*  *おすすめコンテンツ*。多くのアイテムに同じタグが付けられている場合、(フィード内のタグに基づいて行われる) おすすめコンテンツのマッチングにおいて、コンテンツは無制限にマッチングされます(コンテンツマッチングでアイテムの制限を設ける必要があります)。
*  *アプリ内課金コンポーネント。* [アプリ内課金コンポーネント][fire-app-builder-amazon-in-app-purchase-component]を使用している場合、ユーザーがアプリを再起動するかコンテンツの再生を試みるまで、別の端末で購入したアイテムがアプリで認識されません(状態がバックグラウンドに移行したときに、購入したアイテムがアプリによって更新される必要があります)。
*  *スプラッシュ画面。* スプラッシュ画面で最初にフィードをロードするときに時間がかかることがあります(最初のロード時間が短縮される必要があります)。


{% include links.html %}
