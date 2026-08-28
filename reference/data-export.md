
# データのエクスポート

この記事では、Unsubダウンロードのデータフィールドについて説明します。

### Metadata <a href="#metadata" id="metadata"></a>

**issn\_l\_prefixed**

ジャーナルで使用しているプライマリISSN（issn.orgリンクISSN）の先頭に "issn: "を付けたもの。

**issn\_l**

ジャーナルで使用しているプライマリISSN（issn.org リンクISSNをご参照ください。）

**title**

ジャーナルのタイトル

**issns**

このジャーナルのISSNを表すJSON配列

**publisher**

ジャーナルの出版社名。出版社名がわからない場合は "null"。

> **ℹ️ 情報：**
> OpenAlexでは、「コンセプト」（ここでは「サブジェクト」と同じ意味）という用語が使われています。

**subject**

単一のOpenAlexコンセプト(Unsubのsubjectに相当)。コンセプトは、レベルゼロのOpenAlexコンセプトにフィルタリングし、最大スコアを持つものを選択します。複数のコンセプトがある場合は、"A" から始まるアルファベット順で選択されます。このアルファベット順の選択により、subject\_top\_threeも参照することができます。詳しくは[OpenAlexのドキュメント](https://docs.openalex.org/about-the-data/venue#x_concepts)を参照してください。

**subject\_top\_three**

OpenAlexの上位3コンセプト。ジャーナルとコンセプトの関連性の強さのスコアに基づいて、レベル0のOpenAlexコンセプトの上位3つを使用して選択されています。詳しくは[OpenAlexのドキュメント](https://docs.openalex.org/about-the-data/venue#x_concepts)をご覧ください。

**subjects\_all**

OpenAlexのレベル0の全コンセプトとそのIDをJSON配列にしたものです。この ID を使って各コンセプトの詳細情報を<https://openalex.orgに追加すると、調べることができます> (例: <https://openalex.org/C185592680)詳しくは[OpenAlexのドキュメント>]\(<https://docs.openalex.org/about-the-data/venue#x_concepts)をご覧ください。>

### Summary <a href="#summary" id="summary"></a>

**subscribed**

シナリオの中でジャーナルが現在 "subscribed "としてモデル化されている場合は`True`、ジャーナルが現在 "unsubscribed "の場合は`False`

**is\_society\_journal**

学会誌の場合は`True`、学会誌でない場合は`False`。

**usage**

機関が予測したジャーナルの利用状況。利用率は、機関にとってそのジャーナルがどのような価値を持つかを示す指標です。以下の通り計算されます。

`Usage of a journal =`

`Downloads from the journal`

`+ (Citations to the journal by your authors) * (citation weight)`

`+ (Authored papers in the journal) * (authorship weight)`

`ジャーナルの利用＝ジャーナルからのダウンロード＋（所属機関著者のCitations）＊(Citationの重み付け)+（ジャーナル内の著者の論文数）＊(著者の重み付け)`

**cpu**

ジャーナルの利用単価。Unsubではより高度なCPUを使用しています（社内では、これをNet Per Paid Use、またはNCPPUと呼んでいます）。このCPU計算は、Net Cost（購読料からILLを差し引いたもの）をPaid Use（無料ソースで満たせない利用）で割ったものです。これは、購読料に見合う本当の価値を測定したもので、ジャーナルの価値に関する私たちの最も重要な尺度です。詳しくは[こちらの記事](/unsub_guide_jpn/unsubnoshikumi/taitorugotonohadonoyounisurunodesuka.md)をご覧ください。

**cpu\_rank**

データセットに含まれる他のジャーナルと比較した、CPUに応じたジャーナルのランク。費用対効果の高いジャーナルのランクが上位になります。<br>

**cost**

シナリオのジャーナルの設定と購読状況に応じた、ジャーナルのコスト。シナリオでジャーナルが現在購読されているかどうかに応じて、購読コストまたはILLコスト（次のコラムを参照）のいずれかが表示されます。

**instant\_usage\_percent**

現時点で利用可能なオープンアクセス、PTA、サブスクリプションの利用割合

**free\_instant\_usage\_percent**

オープンアクセスまたはPTAで満たされる利用率のパーセンテージ。（ILLまたは購読によってのみ賄われる利用分を除く）

<br>

### Costs <a href="#costs" id="costs"></a>

**subscription\_cost**

ジャーナルタイトルごとの購読料。パラメータ設定による「コンテンツフィー」と、今後5年間の毎年の値上げ分が加味されています。（表示されている金額は、今後5年間の平均費用です）価格をアップロードしていない場合、出版社が公開している価格表の数字が表示されます。詳しくは[こちらの記事](/unsub_guide_jpn/unsubnoshikumi/taitorugotonohadonoyounisurunodesuka.md)をご覧ください。

**ill\_cost**

ジャーナルのILL費用。ILLトランザクションコストとお客様のILLリクエスト率による数値で、いずれも調整可能なパラメータです。詳しくは[こちらの記事](/unsub_guide_jpn/unsubnoshikumi/illrikuesutotoillkosutohadonoyounisurunodesuka.md)をご覧ください。

**subscription\_minus\_ill\_cost**

購読のNet Cost。上記のsubscription\_costからILL費用を差し引いたものです。利用率多くかつ料金の安いジャーナルではマイナスとなることもあり、つまり購読した方が*安く済むということになります。*

### Fulfillment <a href="#fulfillment" id="fulfillment"></a>

**use\_oa\_percent**

グリーン、ハイブリッド、ブロンズのオープンアクセスで賄われる利用の割合。このコンテンツの一部は、設定で除外することができます（詳しくは、オープンアクセスのページをご覧ください）

**use\_backfile\_percent**

PTA (Post-Termination Access：契約満了後アクセス権)により賄われる利用の割合。

\
**use\_subscription\_percent**

タイトルごとの購読によってのみ賄われる利用の割合。（可能な限りオープンアクセスおよびPTAによる要求を実現した後の数値となります。PTAに関しては要データアップロード）

**use\_ill\_percent**

ILL経由で賄われる利用の割合。Turnaway（オープンアクセス、PTA、またはタイトルごとの購読によって満たされない使用）にILLリクエスト率パラメータを掛けたものです。詳しくは[こちらの記事](/unsub_guide_jpn/unsubnoshikumi/illrikuesutotoillkosutohadonoyounisurunodesuka.md)をご覧ください。

**use\_other\_delayed\_percent**

経路が不明な利用の割合。オープンアクセス、PTA権、タイトルごとの購読、ILL、どれにおいても賄われないの利用が計上されます。著者に直接論文を手渡すよう依頼したケース、同僚に論文の共有を依頼したケース、自分の目的に合った別の似た論文を見つけるケース、などが含まれます。

**perpetual\_access\_years\_text**

お客様機関がこのタイトルにPTA（Post-Termination Access）を持っている年数です。デフォルト設定：空欄

\
**baseline\_access\_text**

以前購読していたジャーナルを記入するためのオプション項目。すでにパッケージ契約を終了したお客様向け。

**bronze\_oa\_embargo\_months**

ジャーナルによっては、ある程度の時間が経つと出版社が自動的にコンテンツを無料で読めるようにするものがあります。そのようなジャーナルについて、出版社のサイトで自動的に無料で読めるようになるまでの時間（月単位）をこの欄に記載しています。

### &#x20;Usage Components <a href="#usage-components" id="usage-components"></a>

**downloads**

お客様機関所属の方が論文をダウンロードする回数の予測。COUNTER統計と[ダウンロード減衰曲線に関する文献](https://www.biorxiv.org/content/10.1101/795310v1)（論文が出版されてからどのくらい時間が経過しているかによってダウンロードされる頻度が変わる）を基に算出されます。

**citations**

お客様機関所属の方の執筆論文が当該ジャーナル論文から引用する回数の予測。この数値は過去5年間の引用パターンに基づいています。利用状況全体に対するこの数値の重要度は、Citation Weightパラメータで決定されます。

**authorships**

当該ジャーナルに掲載された論文でお客様機関から少なくとも1名の著者が出ている論文の予測数。この数値は、過去5年間のオーサーシップパターンに基づいています。この数値の重要度は、Authorship Weightパラメータで決定されます。

### Fuzzed <a href="#fuzzed" id="fuzzed"></a>

#### **\*\_fuzzed** <a href="#fuzzed" id="fuzzed"></a>

このデータは正確ではありませんが、おおよそを共有したい場合に備えて、いくつかの「ファジー化」された列を含んでいます。ファジー化された各列では、列内のすべての値をランク付けし、その値を3つの同じ大きさのグループに分けて、低、中、高とラベル付けしています。lowは順位が最も低い値、highは順位が最も高い値、mediumはその中間の値を指します。un-fuzzedの値が存在しない場合は、ダッシュ（"-"）を使用しています。

タイトル間でより細かい解像度が必要な場合は、un-fuzzed列を参照することができます。<br>
