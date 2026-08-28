# パッケージの作成

> **⚠️ 注意：**
> ログインはお済みでしょうか？まだの場合は、[こちら](/unsub_guide_jpn/chtoriaru/roguin.md)を参照にログインしてください。

このページでは、Unsub上でパッケージを作成する方法を説明します。

パッケージとは、ジャーナルの予測シナリオを格納するコンテナのようなものです。パッケージは、出版社もしくはアグリゲーターとの契約を更新するかどうかを検討し始めるときに設定するものとお考えください。Unsub上でのパッケージは、出版社やアグリゲーターの購読パッケージと類似しているものです。

## 1 新規パッケージの作成

&#x20;ご所属の教育機関をクリックします。下の画像は「Demo University」の場合です。複数の教育機関が表示される場合は、パッケージを作成したい教育機関を選んでください。

<figure><img src="/files/cHowQ3ygsbSaxTgN9Dq8" alt=""><figcaption><p>ご所属の教育機関をクリックしてください。</p></figcaption></figure>

まだパッケージが作成されていない場合は、下のボタンが表示されます。最初のパッケージを作成するには、「+ **New package**」をクリックします。

<figure><img src="/files/JWXnAOly2A9iHGK2tTi6" alt=""><figcaption><p>「+New package」をクリックします。</p></figcaption></figure>

**Add subscription package**というタイトルのポップアップウィンドウが表示されます。

<figure><img src="/files/ndaYzvsn1gL88LMXSL14" alt=""><figcaption><p>購読パッケージの追加を行います。</p></figcaption></figure>

パッケージの表示名（必須）を入力します。パッケージの作成には、パッケージ名が必要です。

パッケージの説明（オプション）を入力します。この説明欄には、パッケージの重要な詳細について、同僚やあなた自身を後で思い出すのに役立つような情報をメモしておくことができます。（パッケージ名と説明文は後での変更が可能です。）

その後OKをクリックすると、パッケージが作成されます。パッケージのページでは作成されたすべてのパッケージがリストアップされます。パッケージはいくつでも作成でき、1つのパッケージは1つのパブリッシャーを扱います。

<figure><img src="/files/UHMLUNFMiIm1JnglLvsu" alt=""><figcaption><p>作成したパッケージはこのように表示されます。</p></figcaption></figure>

## 2 パッケージのセットアップ

パッケージの作成が完了したら、次セットアップを行います。

必須項目

* COUNTER準拠利用統計のアップロード
* 価格リストのアップロード
* 通貨（米ドル、英ポンド、日本円）の選択
* ビッグディール（パッケージ契約）にかかっている金額

推奨事項

* 購読終了後アクセス権(PTA:Post Termination Access)の情報アップロード(Excelフォーマット)

オプション事項

* タイトルホワイトリスト

以下は、セットアップを図式化したガイドです。シナリオの詳細についてはこの後のチュートリアルで説明しますが、セットアップの全体像については、このガイドをご覧ください。

<figure><img src="/files/EU5eW8db0OKVPDBecrFI" alt=""><figcaption><p>Unsubセットアップの図ガイド</p></figcaption></figure>

必須項目のファイルと情報がアップロードおよび入力されていることを確認してください。推奨セクションにあるものについてはあるに越したことはないですが、もしこの後で用意できるのであれば、その際にこのページで確認してください。

新規のパッケージは、下図のように表示されます。（4つの必須データタブには赤い❌がついていますが、これはまだ設定する必要があることを示しています）

<figure><img src="/files/QC4S6Ms4GU3GM35YhhSx" alt=""><figcaption><p>必須項目の入力</p></figcaption></figure>

PTAの項目とオプションデータ（Filter）の下に灰色の選択できないタブがそれぞれ1つ存在しますが、これらは上の4つの必須データが用意されるまで、操作することはできません。

### 2.1 COUNTER準拠の利用統計

お客様機関におけるジャーナル単位の利用統計は、Unsubを使った予測を行う上でいちばん重要なデータとなります。

まずはセットアップ画面の左側にある「COUNTER」をクリックします。&#x20;

下図のようなページが表示され、COUNTERデータ・ファイルがまだアップロードされていないことを示す赤いアラートが表示されます。UnsubはCOUNTER 4と5に対応しており、COUNTER 4の場合は1ファイル（JR1）、COUNTER 5の場合は3ファイル（TR\_J2, TR\_J3, TR\_J4）をアップロードします。

次に、ファイルをアップロードします。該当のCOUNTERファイルをクリップのボタンから選択し、それぞれのファイル名が記載された箇所の右側にある上向きの矢印ボタンを押すとファイルのアップロードが開始されます。

<figure><img src="/files/c7kINsOtYhG6MrOox3v5" alt=""><figcaption><p>COUNTERのセットアップページ</p></figcaption></figure>

アップロードしたファイルに問題がある場合、Unsubが通知でお知らせします。

COUNTER準拠利用統計のアップロードの詳細については、[こちら](#21-counterno)をご参照ください。

> **ℹ️ 情報：**
> 他のタブ(Pricelist, Currency, Big Deal Costs)の項目も、COUNTERデータがアップロードされている間に入力することができます。

### 2.2 タイトル価格

次に、左側の「Pricelist」をクリックすると下図のような画面になります。

<figure><img src="/files/fv8YzaA4LVDzeKDmF97C" alt=""><figcaption><p>タイトル価格のセットアップ</p></figcaption></figure>

赤い警告は、価格情報がないジャーナルの数を表示しています。またタイトル価格情報のないジャーナルをリストアップしたファイルをダウンロードすることができます。&#x20;

パッケージ作成の初期段階ではすべてのタイトル価格がそろっていないこともあるかと思いますが、意図せず漏れているタイトルがある場合はVIEW MISSING TITLESのボタンを押下してください。漏れているタイトルのISSN、タイトル、COUNTERデータの概算が記載されたスプレッドシートがダウンロードされますので、今後重要となる価格情報がUnsubにきちんと反映されているかどうかを確認することができます。

この漏れているタイトルのリストを出版社/アグリゲーターの営業担当者に確認し、個々のタイトル/アラカルトの価格を確認してください。

漏れているタイトルの価格情報を入手したら、[こちら](/unsub_guide_jpn/gogaido/taitorunoappurdo.md)を参照し適切な書式を設定してください。

タイトル価格リストファイルの準備が出来たらデバイス上でそのファイルを選択し、右側にある上向きの矢印を押してアップロードしてください。

### 2.3 通貨

次に、画面左側の「Currency」タブを開きます。クリックすると下図のように表示されます。

<figure><img src="/files/ykyLrPXLL8T9NfjkKNqT" alt=""><figcaption></figcaption></figure>

USD（米ドル）、GBP（英ポンド）、JPY（日本円）のいずれかひとつを選択します。ここで選択した通貨によってタイトル価格に使用されるパブリックプライスリストが決定されます。

**注意：** JPYを選択した場合、JPYの価格のない外貨建てのジャーナルは、お客様でJPYに転換し、タイトル毎のISSNと価格を入れる必要があります。

通貨設定の詳細については、[こちら](/unsub_guide_jpn/gogaido/no.md)を参照してください。

### 2.4 Big Deal costs

画面左側の「Big Deal Costs」をクリックすると、下図のように表示されます。

<figure><img src="/files/jXAGHarSZR2I0qQXSbet" alt=""><figcaption></figcaption></figure>

ここではビッグディール（パッケージ契約）の年間コストと、その値上げ率を設定することができます。

詳細については、[こちら](/unsub_guide_jpn/gogaido/biggudrupakkjino.md)をご確認ください。

### 2.5 Perpetual access永続的なアクセス権

この時点で、4つの必須データセクション(COUNTER, Pricelist, Currency, Big Deal Costs)が入力された状態です。この状態でもそのまま[シナリオを作成](/unsub_guide_jpn/chtoriaru/shinariono.md)することはできますが、ここではより正確な推測をするためのオプション入力項目について説明します。この項目は、後から設定することも可能です。

&#x20;画面左側のPTAをクリックすると、下図のように表示されます。

<figure><img src="/files/IgeTNKLbMSiFEAx9ffVv" alt=""><figcaption><p>PTAセットアップのぺージ</p></figcaption></figure>

オレンジの警告は、PTA(Post Termination Access)データのアップロードを推奨しているものです。

もしこの時点でPTAのデータをお持ちでない場合、[PTAデータの収集](/unsub_guide_jpn/gogaido/akusesuptanoarudta.md)と[データのフォーマット](/unsub_guide_jpn/gogaido/ptaakusesunoappurdo.md)方法に関するヒントをご覧ください。

Once you have your PTA file upload it by navigating to the file on your computer, then press the up arrow to the right.&#x20;

PTAファイルの準備が出来たら、デバイス上でそのファイルを選択、画面右側にある上向きの矢印を押下してファイルをアップロードしてください。 PTAファイルのフォーマットとPTAデータのアップロード方法については、[こちら](/unsub_guide_jpn/gogaido/ptaakusesunoappurdo.md)を参照してください。

### 2.6 フィルター

オプションで、パッケージ内のすべてのシナリオに表示されるタイトルを、ジャーナルの「ホワイトリスト」としてフィルタリングすることができます。フィルターを適用した後に気が変わった場合は、セットアップページからファイルを削除すれば、フィルターを適用していないダッシュボードに戻ることができます。

画面の左側にある「フィルター」をクリックすると、下図のように表示されます。

![Journal Filter setup page](/files/HYaBnjUbnefL6iyvLme9)

ジャーナルのフィルタリングについての詳細は、[こちらの記事](/unsub_guide_jpn/gogaido/jnarufirutno.md)をご覧ください。

---

**次のステップ：** パッケージを作成したら、次は[シナリオの作成](tutorials/create-a-scenario.md)です。
