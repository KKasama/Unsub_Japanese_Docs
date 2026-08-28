> For the complete documentation index, see [llms.txt](https://tamaki.gitbook.io/unsub_guide_jpn/llms.txt). Markdown versions of documentation pages are available by appending `.md` to page URLs; this page is available as [Markdown](https://tamaki.gitbook.io/unsub_guide_jpn/yokuaru/taitorunogashitarinisarenainohanazedesuka.md).

# タイトル毎の個別価格が、設定した通りに表示されないのはなぜですか？

**問題:** タイトル価格リスト上で「The Journal of Example Studies」の価格を$1000に設定し、セットアップタブでアップロードしたとしましょう。

しかしシナリオ上で同じジャーナルの価格を見てみると、$1000以上になっています。

**解決策**: アップロードされた価格情報は、現在の年間購読価格を示しています。一方でシナリオに表示される価格情報は、今後５年間の予測価格の平均値です。シナリオ上で扱われるのはすべて5年先の未来の事象です。より詳しく言うと、今後５年間の平均を示しています。

シナリオ内での価格が高くなるのは、今後５年間で価格が上がることが加味されたことによるものです。Unsubではジャーナルの価格上乗せを考慮し、将来の価格を予測しています。この値上げ率は今までの事例に鑑みデフォルトでは８％に設定されています。パーセンテージの変更を行う場合は、ParametersのタブからTitle-by-title subscription cost growthを選択し、０％を含むお客様のご状況に合わせた値上げ率を設定できます。
