
# タイトル価格のアップロード

> **※ 注意：** スクリーンショットはできるだけ日本語を利用しておりますが、機能制限により英語版で提供している箇所もありますので、予めご了承ください。


各ジャーナルのタイトル別価格は、Unsubの主要なデータソースです。これはビッグディール以外でそのジャーナルを個別に購読する場合に支払うコストの情報です。各ジャーナルのタイトル別価格には、2つの情報源があります。

1. **カスタムアップロード価格**: 各ジャーナルのカスタム価格を簡単なスプレッドシートにアップロードすることができます。入力された価格は、各パッケージで設定した通貨での価格として処理されます。
2. **価格なし:** ジャーナルの単体価格をアップロードしていない場合、価格は不明です。全体の予測モデルに与える影響を考慮し、価格情報のないジャーナルは予測対象から除かれます。

> **ℹ️ 情報：**
> 公示価格について: 現在Unsubでは各ジャーナルの単体価格を公開していませんので、[タイトル価格取得のページ](/unsub_guide_jpn/gogaido/taitorunowosuru.md)を参照してください。

各ジャーナルの価格データの出所は、お客様の機関Unsubページでパッケージをクリックし、セットアップタブから「価格リスト」のセクションをクリックすることで確認できます。

ジャーナルのタイトル価格がアップロードされていない場合、以下の2つの画面のうちいずれかが表示されます。

* **COUNTERレポートがアップロードされていない場合**: プライスリストのページ上のこのメッセージでは、価格のデータが必要であることだけが記載されています。


<figure><img src="../images/setup-pricelist-ja.png" alt=""><figcaption><p>価格リストのセットアップ画面</p></figcaption></figure>

* **COUNTERレポートがアップロードされている場合**: プライスリストデータが必要であることと、価格情報が不足しているタイトルの数が表示されます。

<figure><img src="../images/setup-pricelist-ja.png" alt=""><figcaption><p>COUNTERレポートアップロード済みの価格リスト画面</p></figcaption></figure>

「欠落タイトルを表示」をクリックすると、ISSN、タイトル、そのタイトルの COUNTER データのおおよその合計（"counter\_total" というカラム）を含むスプレッドシートがダウンロードされます。これによりUnsub ダッシュボードに価格が反映されていることの重要性をご理解いただけます。counter\_total" カラムは、COUNTER レポートのデータのみを含み、Unsub ダッシュボードで表示される引用や著者のデータは含まれません。ファイルは下図のようなものとなります。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FIQYtyObwnP4nFjerHhGm%252Fprices-setup-view-missing-titles-example.png%3Falt%3Dmedia%26token%3Da5a73ff9-9aa6-4456-bc0c-3804cb930ad2&width=768&dpr=3&quality=100&sign=a0b4d5cfcf2535bc7b889dfbe1b0dc72&sv=3" alt=""><figcaption><p>View Missing Titlesから得られるスプレッドシートの一例</p></figcaption></figure>

価格データの準備ができたら、Unsubに必要なフォーマットは**ISSN**と**Price**のコラムふたつのみです。価格を設定するジャーナルごとに行を追加します。価格はパッケージ設定で設定した通貨での価格として処理されます。（シート上に入力された通貨は無視されます）.csv、.xlsx、.xlsの3つの形式に対応しており、シートは一枚のみである必要があります。ファイルには、数式やその他の値以外の内容を含めることはできず、またフォーミュラなど数式などの値でない内容を含んだファイルは非対応となります。下図より、ファイルの作成例をご確認ください。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FjWYr4tXwXNGFQVOpgIUu%252FScreen%2520Shot%25202022-10-19%2520at%25209.44.07%2520AM.png%3Falt%3Dmedia%26token%3D1db4377b-d165-4d78-9a72-e32791454d43&width=768&dpr=3&quality=100&sign=71846101dd772a71ef5dde0305cbd12b&sv=3" alt=""><figcaption><p>価格リストのファイル作成例</p></figcaption></figure>

> **🚨 重要：**
> 価格欄にはカンマやピリオドなどの区切り文字を使用しないでください。

まずアップロードボタンをクリックし、クリップのアイコンをクリックします。該当のファイルを選択して矢印をクリックすると1、2分後にアップロードの処理が完了します。アップロード後、下記のような画面が表示されます。

<figure><img src="../images/setup-pricelist-ja.png" alt=""><figcaption><p>価格リストのセットアップ（COUNTERレポートと、一部の価格がアップロードされた状態）</p></figcaption></figure>

アップロードした価格を確認したい場合は、ファイル列の右端にあるダウンロードボタンをクリックします。既にアップロードされているジャーナル価格表を差し替えたい場合は、ファイル行の右側にあるゴミ箱をクリックし、新しいファイルをアップロードしてください。

赤のアラートがオレンジのアラートに変わるのは、必要なデータはアップロードされているが、価格の不足がまだあることを示しています。

すべてのタイトル価格を取得することができた場合、以下の画面のように緑色のアラートとチェックマークが表示されます。

![](https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FIMv066FkNfvtzqw0FfSF%252Fprices-setup-with-counter-withcompletecustom.png%3Falt%3Dmedia%26token%3D663f661e-e566-4c3b-83a5-c2ec3f7abd4f&width=768&dpr=3&quality=100&sign=088cde5d6074385610142c5ef1f62f05&sv=3)

> **ℹ️ 情報：**
> Unsubはジャーナル単位の価格設定にのみ対応しています。ミニバンドル価格への対応については、[こちら](/unsub_guide_jpn/gogaido/minibandoruno.md)をご覧ください。
