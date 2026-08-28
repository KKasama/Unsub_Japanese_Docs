> For the complete documentation index, see [llms.txt](https://tamaki.gitbook.io/unsub_guide_jpn/llms.txt). Markdown versions of documentation pages are available by appending `.md` to page URLs; this page is available as [Markdown](https://tamaki.gitbook.io/unsub_guide_jpn/gogaido/saretataitorurepto.md).

# 除外されたタイトルレポート

COUNTERレポートファイルにアップロードしたすべてのタイトルがUnsubのダッシュボード上に反映されないことがあります。[こちらのページ](/unsub_guide_jpn/yokuaru/notaitorugasarenainohanazedesuka.md)で、タイトルが除外される4つの主な理由を詳しく説明しています。

パッケージの「Setup」タブの「Diagnostic data」セクションに、スプレッドシートをダウンロードできるExcluded Titlesのページがあります。

スプレッドシートには、2つの情報列（issn\_l、publisher）と、タイトルがシナリオから除外される4つの理由を示す4つの列があります。列は次のとおりです。

* **issn\_l**: リンク先のISSN、またはISSN-L
* **publisher**: [OpenAlex](https://openalex.org/)による出版社情報
* **gold\_oa**: `True` OpenAlexがそのジャーナルをゴールド・オープン・アクセス（OA）であると考える場合はTrue、そうでない場合はFalse。購読アクセスルートがないため、ゴールドOAのタイトルを含めることはできません。
* **not\_currently\_publishing**: `True` OpenAlexがそのジャーナルがもう出版されていないと判断した場合はTrue、そうでない場合はFalseです。この判断は、OpenAlexのデータに基づいています。
* **price\_not\_available**: `True` タイトル価格がない場合はTrue、そうでない場合はFalse。タイトル価格をアップロードすることで修正できます。ダッシュボードに含まれるタイトルには、タイトル価格が必要です。
* **filtered\_out**: `True`オプションのジャーナル・フィルタ設定ステップを使用してタイトルをフィルタリングした場合は True、そうでない場合は False。ジャーナル・フィルタリングについてはこちらをご覧ください。

下図はダウンロードするレポートの例です。

<table><thead><tr><th width="137">issn_l</th><th width="105">publisher</th><th width="95">gold_oa</th><th width="166">not_currently_publishing</th><th>price_not_available</th><th>filtered_out</th></tr></thead><tbody><tr><td>2053-9711</td><td>OUP</td><td>True</td><td>False</td><td>False</td><td>False</td></tr><tr><td>0007-0912</td><td>Elsevier</td><td>False</td><td>False</td><td>True</td><td>False</td></tr><tr><td>1473-6691</td><td>SAGE</td><td>False</td><td>False</td><td>True</td><td>False</td></tr><tr><td>0024-6093</td><td>Wiley</td><td>False</td><td>True</td><td>False</td><td>False</td></tr></tbody></table>

データについての注意点

* レポートの4つの列で、スプレッドシートのフィルターツールを使って、同じ理由（例：タイトル価格の欠落）で除外されたすべてのタイトルにフィルターをかけることで、当該のタイトルを調べることができます。
* タイトルが除外される理由はひとつではないこともあります。例えば、ゴールドOAでかつタイトル価格がないという場合がそれに含まれます。
* ダッシュボードにないタイトルを表示させるようにするためには、ひとつの作業で問題が解決することもあります。仮にそのタイトルの価格が欠落している場合、価格情報をアップロードすれば問題は解決します。そのタイトルがフィルタリングされている場合、フィルタリングリストから当該のタイトルを削除することで問題は解決します。ただし、タイトルがゴールドOAだったり、絶版になっている場合は、ダッシュボードに表示させることはできません。
* OpenAlexについてのより詳しい情報は、[OpenAlexのドキュメンテーション(英語)](https://docs.openalex.org/)をご覧ください。

シナリオに含めるべきと思われるタイトルがもしあれば、<support@unsub.org>にご連絡ください。
