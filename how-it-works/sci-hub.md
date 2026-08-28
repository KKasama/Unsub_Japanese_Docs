> For the complete documentation index, see [llms.txt](https://tamaki.gitbook.io/unsub_guide_jpn/llms.txt). Markdown versions of documentation pages are available by appending `.md` to page URLs; this page is available as [Markdown](https://tamaki.gitbook.io/unsub_guide_jpn/unsubnoshikumi/unsubhasci-hubnowoshiteirunodesuka.md).

# UnsubはSci-Hubの利用を考慮しているのですか？

Unsub Scenario Viewは、様々なデータ入力とパラメータ設定に基づいたFulfillment（実現可能性）を視覚化するのに役立ちます。

Fulfillment（実現可能性）の「Unknown」部分（下図参照）は、特にタイトルごとの購読を追加していない場合、いくつかのシナリオでFulfillmentの重要な部分となる可能性があります。Fulfillmentの「Unknown」グレー部分は、基本的に「読者自らの力による入手」となります。

<figure><img src="/files/FEDHyAM0kSnlUzcghmcr" alt=""><figcaption></figcaption></figure>

「読者が自力で」というのは、論文の著者にPDFをもらう、同僚にPDFをもらう、さらにはSci-Hubを使うなど、いろいろな意味があります。

このグレーのUnknownの部分のフルフィルメントでUnsubがSci-Hubを占めているのか気になるところですが、答えはYesです。

UnsubはSci-Hubの利用を考慮していますが、明示的ではありません。Unsubには「ILL Request Rate」というパラメータがあります（ILL Request Rateパラメータについては、[こちら](https://docs.unsub.org/reference/scenarios/scenario-parameters)と[こちら](https://docs.unsub.org/how-it-works/how-do-we-calculate-ill-requests-and-ill-cost)をご覧ください）このパラメータはデフォルトで5%となっています。つまり、ある論文が読者に求められる20回に1回の割合でILLリクエストが発生するということで、Sci-Hubの利用が増えれば、この比率は下がると思われます。

間接的にSci-Hubの利用レベルの違いをモデル化するやり方として、ILL Request Rateパラメータを変更し、異なるILL Request Rate値で異なるUnsubシナリオを比較する方法が挙げられます。
