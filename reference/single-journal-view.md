
# 個別ジャーナルの閲覧

> **※ 注意：** このページのスクリーンショットは英語版です。実際の画面は日本語で表示されます。


シナリオ画面のヒストグラムまたはテーブルビューで任意のジャーナルをクリックすると、単一ジャーナルビューを表示することができます。

下図のジャーナル ”Chest” のボックスをクリックすると、単一ジャーナル表示になります。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FsAuZqTnlUn95s8Fi3nTD%252Fsingle-journal-view-click.png%3Falt%3Dmedia%26token%3Da73c516f-2db8-444e-ad20-21666731fe8b&width=768&dpr=3&quality=100&sign=3e63cb96b1e75790f7c2048a893069f8&sv=3" alt=""><figcaption></figcaption></figure>

こうすることで、タイトルの詳細が表示されます。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FGmBY2vBmmu4ZqQw1QYZV%252Fsingle-journal-view-zoomed.png%3Falt%3Dmedia%26token%3D6c8bd7d3-3e47-4253-ae62-cd1559d6e5f2&width=768&dpr=3&quality=100&sign=ef42e48ca9c675ff7e257f59380581c9&sv=3" alt=""><figcaption></figcaption></figure>

個別タイトルの詳細画面で、ジャーナルのメタデータと[Cost Per Use](/unsub_guide_jpn/refarensu/li-yong-jinecost-per-use.md)の計算の内訳が表示され、購読の設定/解除ができます。

### Overviewタブ

Overviewタブには、ジャーナルメタデータ、年間利用統計、コスト、CPU値が表示されます。

#### Journal metadata

このセクションは、以下を含みます。

* Subject: OpenAlexの"コンセプト"から抽出された、ジャーナルの分野を表示します。詳しくは[こちらの記事](/unsub_guide_jpn/refarensu/dtanoekusupto.md)をご覧ください。
* ISSN: ジャーナルに紐づいているISSN (もしくはISSN-L)
* Society Journal: 当該ジャーナルがSociety Journalの場合は"Yes"、そうでない場合は"No"と表示されます。 &#x20;
* Delayed OA: 当該ジャーナルが遅延OAジャーナルの場合は"Yes"、そうでない場合は"No"と表示されます。Yesの場合、エンバーゴ期間終了後は当該ジャーナルのコンテンツがフリーになります。この場合"OA embargo length"の別項目が表示され、月単位でその期間が表示されます。
* PTA (Post-Termination Access) rights: この項目はPTAデータをアップロードしていない場合空欄となります。アップロードが済んでいる場合、購読後アクセス権の機関が表示されます。

> **🚨 重要：**
> 数値は四捨五入されています。ご自身で計算されると、表示されている数値とは多少の誤差が生じることがありますが、これはすべてUnsub側で四捨五入していることが原因です。ご不明な点がありましたら、<support@unsub.org>までご連絡ください。

> **ℹ️ 情報：**
> 表示されている予測の数値ですので、現在の統計の数値とは異なります。

#### Annual usage

3つの項目があり、一部は重み付けされています。

* Downloads: COUNTER上の統計データから予測される推定ダウンロード回数
* Citations: お客様機関のメンバーが発表した論文上で、当該ジャーナルからの推定引用数
* Authorships: 当該ジャーナルへの、お客様機関メンバーからの推定投稿数

無料での論文利用を含めてしまうと正確なCost per Useが出ないので、Paywalled uses(実際にお金をかけて利用されている回数)を算出します。これを求めるには、Weighted overall usesから下記の項目を差し引きます。

* Open access usage: オープンアクセスコンテンツの推定利用数
* PTA/Backfile usage: PTAおよびバックファイルの推定利用数

#### Annual cost

ジャーナルの個別購読にかかるコストは単純ではありません。Unsubでは、もし購読しなかった場合に発生するILLの費用も考慮します。そのコストであるNet subscription cost&#x306F;**、**&#x57FA;本購読料とILLの見込みコストの差額となります。

#### Cost Per Use

Cost Per Useは、Net subscription costをPaywalled usesの数で割った額となります。

### Timelinesタブ

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FytSxuY7mr8JhxHkqV2ab%252Fsingle-journal-view-zoomed-timeline.png%3Falt%3Dmedia%26token%3Dcf0ecd20-3329-413e-9ae8-30fa4ae9d6ce&width=768&dpr=3&quality=100&sign=580cb4540b74ef3c83fe1ccb6b8e3d08&sv=3" alt=""><figcaption></figcaption></figure>

Timelinesタブには、いくつかのセクションがあります。

* Fulfillment: 当該ジャーナル利用の予測内訳
* Open Access: OAによる利用の予測内訳
* Impact: ダウンロード、引用、投稿の数を計上した予測利用回数
* Subscription cost: 年ごとの予測購読費用
* API response: [JSON](https://en.wikipedia.org/wiki/JSON)フォーマットのレスポンス（技術者向け）
