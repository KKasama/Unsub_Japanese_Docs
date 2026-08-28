
# COUNTER準拠の統計アップロード

> **※ 注意：** このページのスクリーンショットは英語版です。実際の画面は日本語で表示されます。


Unsubを使用して購読の分析と予測を行う前に、お客様のCOUNTERデータをアップロードする必要があります。Unsubはこのデータを使って、予測モデルをお客様の機関に合わせてカスタマイズします。&#x20;

まず、パッケージのセットアップに移動します。COUNTERタブは以下のように表示されます。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FWaHKiGLGcc7A09LtGRY9%252Fupload-counter-data-not-loaded.png%3Falt%3Dmedia%26token%3D4e8f9518-5a11-47c2-8d0a-82bd2f231b9c&width=768&dpr=3&quality=100&sign=ef9bf36209725541eecdc87b2cffa99b&sv=3" alt=""><figcaption></figcaption></figure>

COUNTER 4も引き続きサポートされていますが、新しいパッケージにはCOUNTER 5データを使うことをお勧めします。&#x20;

既にCOUNTER 4のデータがアップロードされている場合、右側のゴミ箱アイコンをクリックしてそのファイルを削除したのちにCOUNTER 5のポッチを選択し、COUNTER 5の統計データをアップロードしてください。こうすることで、簡単に新しいデータと差し替えることができます。差し替えが済んだ後はすべての予測シナリオの計算に新しいデータが適用され、予測内容は自動的に更新されます。

COUNTERファイルを準備する際、以下の点に注意してください。

* COUNTER 5の場合、3つのファイル(TR\_J2、TR\_J3、TR\_J4)が必要となります。（COUNTER 4の場合はJR1のひとつのみとなります）
* &#x20;If you can not get a TR\_J2 file or the TR\_J2 file does not have any rows of data except the header rows you can download and use [this fake **TR\_J2** file](https://unsub-public.s3.amazonaws.com/TR_J2.csv). It should not affect your dashboard.過去のお客様事例に鑑みると、TR*J3とTR*\_J4ファイルはほとんど問題なく入手できますが、TR\_J2は入手できない、もしくはデータ行が存在しない場合があるようです。TR\_J2のファイルが入手できないあるいはTR\_J2ファイルにヘッダー行以外のデータ行がない場合は、[こちら](https://unsub-public.s3.amazonaws.com/TR_J2.csv)からモックTR\_J2ファイルをダウンロードしご利用ください。ダッシュボードの予測に影響を与えることはありませんので、ご安心ください。&#x20;
* csv、.xls、および .xlsxのファイル形式のみがサポートされています。
* アップロードするファイルには、一枚目のシートにすべての情報を記載するようにしてください。
* COUNTERデータは12ヶ月分の使用量を想定しています。連続した12ヶ月間のものならどのようなものでもご利用いただけます。前の年の4月からのもの、またもし前の年の利用が例年とは大きく異なる場合その前の年の4月からのものでも問題ありません。
* COUNTERファイルには、計算式やその他の値以外の内容を含めることはできません。Unsubでは、数式などの非数値的な内容を含むファイルは非対応となります。

COUNTER準拠の利用統計ファイルが手元にあれば、アップロードを開始する準備は完了です。クリップのアイコンをクリックしてCOUNTERファイルを選択し、上向きの矢印ボタンをクリックします。

システムがファイルのアップロードを開始し、処理には数分を要します。アップロードが完了すると、下図のような画面が表示されます。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FtIYSqiE2nURJyr6094hr%252Fupload-counter-data-fully-loaded.png%3Falt%3Dmedia%26token%3Dfbf80b53-3ff7-4e36-8395-e07c13026cbc&width=768&dpr=3&quality=100&sign=134e9a57af09ee83382e205e3d6c5bcc&sv=3" alt=""><figcaption></figcaption></figure>

各ファイルの右端にあるダウンロードの矢印をクリックすると、保存されているデータを確認することができます。このデータを後で置き換えたい場合は、行の右側にあるゴミ箱をクリックし、新しいファイルをアップロードしてください。シナリオ予測は自動的に新しいデータを使って再計算されます。&#x20;

COUNTERファイルにはオープンアクセスジャーナルや出版中止のジャーナルが含まれているため、ファイル内のすべてのジャーナルが予測ダッシュボードに表示されるわけではないことにご注意ください。また価格データが欠落している場合、当該のジャーナルは統計内に利用の記録が予測対象に入りません。（この問題を修正するには、[こちら](/unsub_guide_jpn/gogaido/taitorunoappurdo.md)をご参照ください。）

<br>
