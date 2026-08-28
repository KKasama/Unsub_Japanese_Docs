
# UnsubはSci-Hubの利用を考慮しているのですか？

> **※ 注意：** このページのスクリーンショットは英語版です。実際の画面は日本語で表示されます。


Unsub Scenario Viewは、様々なデータ入力とパラメータ設定に基づいたFulfillment（実現可能性）を視覚化するのに役立ちます。

Fulfillment（実現可能性）の「Unknown」部分（下図参照）は、特にタイトルごとの購読を追加していない場合、いくつかのシナリオでFulfillmentの重要な部分となる可能性があります。Fulfillmentの「Unknown」グレー部分は、基本的に「読者自らの力による入手」となります。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FbUv6AGdjtt2bCUheahLT%252Faccount-for-scihub.png%3Falt%3Dmedia%26token%3Dc9e480b3-51c5-4141-bac7-01df3a2c68a5&width=768&dpr=3&quality=100&sign=7bf77521713bc3adfe5de8af25d5df61&sv=3" alt=""><figcaption></figcaption></figure>

「読者が自力で」というのは、論文の著者にPDFをもらう、同僚にPDFをもらう、さらにはSci-Hubを使うなど、いろいろな意味があります。

このグレーのUnknownの部分のフルフィルメントでUnsubがSci-Hubを占めているのか気になるところですが、答えはYesです。

UnsubはSci-Hubの利用を考慮していますが、明示的ではありません。Unsubには「ILL Request Rate」というパラメータがあります（ILL Request Rateパラメータについては、[こちら](https://docs.unsub.org/reference/scenarios/scenario-parameters)と[こちら](https://docs.unsub.org/how-it-works/how-do-we-calculate-ill-requests-and-ill-cost)をご覧ください）このパラメータはデフォルトで5%となっています。つまり、ある論文が読者に求められる20回に1回の割合でILLリクエストが発生するということで、Sci-Hubの利用が増えれば、この比率は下がると思われます。

間接的にSci-Hubの利用レベルの違いをモデル化するやり方として、ILL Request Rateパラメータを変更し、異なるILL Request Rate値で異なるUnsubシナリオを比較する方法が挙げられます。
