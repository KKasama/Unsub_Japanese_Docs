
# ジャーナルフィルターの追加

> **※ 注意：** このページのスクリーンショットは英語版です。実際の画面は日本語で表示されます。


はじめUnsubはダッシュボード1つに対し1つの出版社のコンテンツにのみ対応していました。例えばElsevier社のCOUNTERレポートをアップロードすると、ダッシュボードにはElsevier社のジャーナルしか表示されませんでしたが、現在はあらゆる出版社のジャーナルを1つのダッシュボードにまとめられるようになりました。

現在のUnsubは、あらゆる出版社のタイトルに対応しており、ダッシュボードで出版社ごとにタイトルをフィルターする必要はなくなりました。 アップロードしたCOUNTERレポートには、[これらの理由](/unsub_guide_jpn/yokuaru/notaitorugasarenainohanazedesuka.md)に該当しない限りすべてのタイトルが表示されます。

&#x20;出版社単位でのフィルタリングに替わるものとして、オプションでユーザーによるタイトル・フィルタリングを導入しました。

### Filtering titles

最初にパッケージに移動し、「Setup」タブをクリックし、「Filter」セクションまでスクロールします。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FeStUxwKm3mu5hBlI3oW1%252Fupload-journal-filter-not-uploaded.png%3Falt%3Dmedia%26token%3D5eff6f24-1af5-43b2-b55a-343e711babef&width=768&dpr=3&quality=100&sign=105a3249e2b16eac9873855379e777fb&sv=3" alt=""><figcaption><p>フィルターセットアップが行われる前の状態</p></figcaption></figure>

水色のアラートはデータがアップロードできることを示しています。

KBARTファイルをアップロードする場合は、ホワイトリストに登録したいISSNのみにファイルを編集してください。

カスタムファイルをアップロードします。ファイルはとてもシンプルで、下図のようにISSNカラムひとつのみのスプレッドシートです。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FG6ojg0BeuaN3i9aonNNq%252Fupload-journal-fliter-example-file.png%3Falt%3Dmedia%26token%3D2fb52b00-e736-4fe6-80d0-1e30a431de30&width=768&dpr=3&quality=100&sign=592e2db490bcacc7dad8f5564b8cbefc&sv=3" alt=""><figcaption></figcaption></figure>

クリップのアイコンをクリックし、該当のファイルを探して選択します。上向きの矢印をクリックするとアップロードが始まり、処理におよそ1～2分ほど要します。完了すると、下のような画面が表示されます。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FWhP2mAZQTo3odEX1RwVv%252Fupload-journal-filter-uploaded.png%3Falt%3Dmedia%26token%3Db6393289-5684-4f96-a847-299c84eb0be1&width=768&dpr=3&quality=100&sign=8eb638742471b995809ad80c42a286f2&sv=3" alt=""><figcaption></figcaption></figure>

上の図を見ると、250行のデータがあることがわかります。画面右側にある下向きの矢印をクリックすると、フィルターしたジャーナルの一覧をダウンロードできます。

データを後で差し替えたい場合は、画面右にあるゴミ箱のアイコンをクリックし、新しいファイルをアップロードしてください。&#x20;

パッケージ内のシナリオに戻ると、以下のように右上に "Journal Whitelist (数字) "という青いメッセージが表示されます。

<figure><img src="https://docs.unsub.org/~gitbook/image?url=https%3A%2F%2F2329511114-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FeIwtiPevlQYuy1bQ4x85%252Fuploads%252FvtIXzw0SoVppFfgonY1S%252Fupload-journal-filter-uploaded-resulting-scenario.png%3Falt%3Dmedia%26token%3D5b7324cd-7b86-4b3d-998f-3ae863c98af0&width=768&dpr=3&quality=100&sign=3f1ded2a27b3a1124d9ceee4e97a7a8f&sv=3" alt=""><figcaption><p>フィルター機能を利用したシナリオ</p></figcaption></figure>

青い字でJournal Whitelistと書かれた箇所をクリックすると、このドキュメント・ページにアクセスできます。

なお以下のような状況では、ダッシュボードに表示されるタイトルとフィルターの設定ステップでアップロードしたタイトルとが完全に一致しない場合がありますのでご注意ください。

* シナリオのタイトル数が変わらないケース。（この場合、フィルタリングしたタイトルがダッシュボードに表示されているタイトルと完全に一致している可能性が考えられます）&#x20;
* シナリオ内のタイトル数は減ったが、まだいくつかのタイトルが残っているケース。（最も一般的なケースです）
* ダッシュボードにタイトルがない。これは、有効なISSNでフィルタリングしても、ダッシュボード上のどのタイトルとも一致しなかった場合に発生し得ます。

上記どのケースでもない場合、またもしご質問がありましたら<support@unsub.org>までご連絡ください。
