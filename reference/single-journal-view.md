
# 個別ジャーナルの閲覧

シナリオ画面のヒストグラムまたはテーブルビューで任意のジャーナルをクリックすると、単一ジャーナルビューを表示することができます。

下図のジャーナル ”Chest” のボックスをクリックすると、単一ジャーナル表示になります。

<figure><img src="/files/uiDx2bA8Jd7hBswckv7W" alt=""><figcaption></figcaption></figure>

こうすることで、タイトルの詳細が表示されます。

<figure><img src="/files/mmvRaweeaBo326aQxvXP" alt=""><figcaption></figcaption></figure>

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

{% hint style="danger" %}
数値は四捨五入されています。ご自身で計算されると、表示されている数値とは多少の誤差が生じることがありますが、これはすべてUnsub側で四捨五入していることが原因です。ご不明な点がありましたら、<support@unsub.org>までご連絡ください。
{% endhint %}

{% hint style="info" %}
表示されている予測の数値ですので、現在の統計の数値とは異なります。
{% endhint %}

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

<figure><img src="/files/f4wTIWjKu9RZgyHEn7Ea" alt=""><figcaption></figcaption></figure>

Timelinesタブには、いくつかのセクションがあります。

* Fulfillment: 当該ジャーナル利用の予測内訳
* Open Access: OAによる利用の予測内訳
* Impact: ダウンロード、引用、投稿の数を計上した予測利用回数
* Subscription cost: 年ごとの予測購読費用
* API response: [JSON](https://en.wikipedia.org/wiki/JSON)フォーマットのレスポンス（技術者向け）
