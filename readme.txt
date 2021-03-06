>---------------------------------------------------------<
　Dancing★Onigiri エディター　Ver3.3.1
　＋ Score Revival (譜面復元ツール) Ver1.2.0
>--------------------------------------------------------<

Dan★Oniの7keyエディターを基に、
ティックルが他のキー用に拡張したエディターです。

上記エディターのセーブデータを復元する、
Score Revivalも同梱しています。

>---------------------------------------------------------<

▽　入っているもの

・　[editor]
　　 ├ editor.exe		(エディター本体)
　　 ├ editor_wide.exe		(エディター本体・縦長版)
　　 ├ ini.txt			(ショートカットキー割当設定用ファイル＋その説明）
     ├ keys.txt　　　　       （譜面名前変更用ファイル＋その説明）
　　 ├ optionEdit2.swf		(Option Editor 2)
     └ [src]			
　　 　　├ editor.fla		(Flash CS6に対応したソース)
　　　　 └ editor.swf		(Dan☆Oniソース内包swfファイル)
				　　※通常のエディターとして使うこともできます
　　 　　├ editor_wide.fla	(Flash CS6に対応したソース・縦長版)
　　　　 └ editor_wide.swf	(Dan☆Oniソース内包swfファイル・縦長版)

・　[scoreRevival]
　　 └ scoreRevival.exe	(譜面復元ツール)

・　Dan★Oniエディター ヘルプ.chm　(ヘルプ)
・　history.txt		（更新履歴）
・　keys_format.txt　　　(デフォルトで設定されているkeys.txtの情報。参考資料)
・　readme.txt　　　　  （要するにコレ）

>---------------------------------------------------------<

▼　元に戻す/やり直す[Undo/Redo]機能 (Ver3.0.0〜)

コマ操作(3連符変換コマ、コマ一括操作を除く)について
操作を1つ戻す、1つ進むことができるようになりました。

画面に表示されていないコマの操作があった場合は
対象のコマのページで飛んでからコマの削除・追加を行います。
速度コマについても元に戻せますが、速度は1に戻るのでご注意ください。

コマ一括操作(カット、ペースト、押し下げなど)を行うと、
Undo/Redoがリセットされます。
必要な場合は、事前にSAVEするなど退避することをお勧めします。


▼　クイックセーブ・ロードについて (Ver3.0.0〜)

FlashのSharedObjectの機能を使って、
セーブデータのローカル保存ができるようになりました。
データの一時退避を目的に、最大10個まで用意しています。

　・シフトキーを押しながら「SAVE」ボタンを押す
　・右上「×」ボタンの後に「セーブ」ボタンを押す
という操作を行うことでセーブ画面が現れるので、保存したいところで「SAVE」します。
左側のテキストボックスには、譜面を区別するためのメモを入れることができます。

ロードする場合は、「ふっかつのじゅもん」の画面から
「solデータからQロード」の部分をクリックしてください。


▼　メニュー配置の一部変更 (Ver3.0.0〜)

譜面番号、表示切替ボタンについてはオプション画面に移動しました。

>---------------------------------------------------------<


▽　範囲指定コピー・ペースト (Ver2.13.0〜)

　　任意の範囲(小節単位)を指定してコピー・ペーストができるようになりました。
　　範囲指定のボックスにチェックを入れて、開始と終了を指定後、
　　　「Z」＋「X」：カット
　　　「Z」＋「C」：コピー
　　　「Z」＋「V」：上書きペースト
　　　「Z」＋「B」：重ねペースト
　　で可能です。右クリックメニューに対応しています。

　　コピー範囲が1ページを超えるものも可能になるため、
　　ペースト時、ペースト先に譜面があれば警告を入れるようにしました。
　　ペースト先に譜面がなければ、無条件で貼り付けます。


▽　縦長版エディターについて (Ver2.10.2〜)

　　縦長版と通常版のセーブデータは互換性があります。
　　通常のエディターと同様に使うことができます。


▽　譜面の多重読み込みについて (Ver2.9.0〜)

　　エディターのメイン画面から、複数譜面を読み込めるようになりました。
　　1〜5のボタンで譜面を切り替え、必要に応じて「LOAD」で読込。
　　これにより、譜面間の比較・コピー＆ペーストが可能になりました。
　　※セーブデータは各譜面で独立しています。変更した譜面のセーブ忘れに注意してください。


▽　背景の設定について (Ver2.8.5〜)

　　[img]フォルダに背景画像(450x400サイズ)を入れるとエディター起動時に反映されます。
　　ただし、ファイル名に制限があります。拡張子は「jpg」と「png」にのみ対応しています。
　　　・1ファイル目：image.jpg
　　　・2ファイル目：image1.jpg
　　　・3ファイル目：image2.jpg
　　　　　：

　　背景画像の変更はエディタータイトルの「BACK」ボタンから変更可能です。

▽　Interval(4分間隔)調整機能について (Ver2.8.0〜)

　　Editorメインにある、Intervalの欄の横に
　　「↑」「↓」ボタンを追加しています。
　　対象位置基準で、フレームの終了位置を変化させることで
　　Intervalの調整を行います。
　　テンポ変化がない場合は、譜面の全体ズレの修正が容易になります。
　　
　　具体的には次のように使います。

　　例) FirstNumber :200, Interval: 10
　　　　FirstNumberは合っていて、13ページ目開始時点で2フレーム早いことが分かったとき：

　　　　12ページ目先頭にページを移し、「↓」(タイミングを遅くする)ボタンを2度押す。
　　　　　200 〜 4040フレーム    (Interval : 10)
　　　　　→ 200 〜 4042フレーム (Interval : 10.0052)

　※ Score Correctorとは異なり、テンポ変化している場合は
　　 変更対象が絡んでいるIntervalのみ変更します。

　　例) FirstNumber :200,  Interval: 10 (〜10ページ目まで)
　　　  FirstNumber :3400, Interval: 10 (11ページ以降)
　　　　FirstNumberは合っていて、13ページ目開始時点で2フレーム早いことが分かったとき：

　　　　上記と同じ操作を行うと次のようになります。
　　　　＜〜10ページ目まで＞　→　変更なし　　　　　　 (Interval : 10)
　　　　＜11ページ目以降＞　　→　3400 〜 4042フレーム (Interval : 10.03126)

　※ シフトを押しながら「↑」「↓」ボタンを押すと、0.25フレーム単位の調整になります。


▽　Option Editor 2の呼び出しについて (Ver2.6.6〜)

　　Editorメイン -> オプション(2ページ目)のヘッダー情報に
　　「読込」ボタンが増えています。
　　editor.exeと同じ場所に"optionEdit2.swf"がいれば、
　　「読込」ボタンを押すことで「Option Editor 2」が起動します。

　　必要データを入力後、「出力」ボタン→「続行」を押すと
　　エディター画面に戻ります。
　　このとき、「読込」ボタンが「書出」になっていると思います。
　　この状態で「書出」を押すと、
　　「Option Editor 2」で設定した内容がヘッダーに反映されます。


▽　ヘッダー、フッター取込/出力 (Ver2.6.0〜)

ヘッダー・フッターの取込に対応しました。
対応している変数名は次の通りです。

　ヘッダー：　musicTitle, difData, difStep, difName, speedlock, setColor, frzColor, startFrame, headerUrl, editorUrl
　フッター：　color_data, acolor_data, word_data
　　　　　　　※指定された譜面番号にあったものが取込対象

またヘッダー・フッターの取込対象を増やしたい場合、
"keys.txt"の以下の変数に書き込むことによりカスタマイズ可能です。

　ヘッダー： headerVal 　　　例) &headerVal=musicNo,version&	※カンマ区切り
　フッター： footerVal

※外部エディターへの対応

　　・FUJIさんエディター　　：ヘッダー、フッターをそのまま入出力するため問題なし。
　　・ドイルさんエディター　：ヘッダーのみ対応。セーブデータの仕様上、以下の変数しか利用できない。
			　　　musicTitle, difStep, difName, speedlock


▽　フリーズアロー・個別加速の指定方法について（重要）

これまで、矢印コマ・スピードコマを2回クリックする必要がありましたが、
Ver2.44以降は「シフトを押しながら」矢印コマ・スピードコマを1回クリックします。


▽　keys.txtについて(重要)

エディターと同じ場所にこのファイルを置いて下さい。
これが無くても動きますが、
変則キー(11i, 12, 13, 14i, 17key)が使用できなくなります。

また、従来のテンプレートに相当する機能を持っており、
キー拡張も可能です。
詳細はヘルプを参照してください。

良く使うキーは、keys.txtの中にある

　&keyList=5,7,7i,9,11,11i,12,13,14i,15,17&

の順序を変えたり、必要分のみにしておくと使い勝手が良くなるかもしれません。
例えばこんな感じに。

　&keyList=7,11,15,7i,5,9,17&


▽　各種エディター対応状況

　・ドイルさんエディター
　　　⇒ テンポ変化はページ単位のため、
　　　　 ページの途中でテンポ変化(Fix)すると正しく取込できません。
　　　　 エクスポートする場合、テンポ変化位置がページの先頭になるよう調整してください。

　・FUJIさんエディター
　　　⇒ テンポ変化はページ途中でも可能です。
　　　　 ただし、1小節単位(16コマ1セット)のテンポ変化にする必要があります。
　　　　 3拍子、5拍子、7拍子は拍飛ばしにも対応。

　・ステマニエディター(読込限定)
　　　⇒ テンポ変化に対応。
　　　　 他のエディターと異なり、小節間のテンポ変化があっても読み込めます。
　　　　 ただし小節間に置いた場合、テンポ変化位置の変更ができないため注意が必要です。
　　　　 ファーストナンバー等は、小節を挟めば変更が可能です。

▽　トラブルシューティング

　　・　「GO」を押して重くなった場合は：
	計算中のため重くなっているだけなので、落ち着くまで一旦放置してください。
	「スクリプトの関係で処理が遅く〜」となってもとりあえず実行で。
	何度もボタンを押すと逆に失敗します。

　　・　Score Revivalの詳細はヘルプをご覧ください。
　　　　簡単な内容であれば、Score Revival本体右上の「？」でも確認できます。

>---------------------------------------------------------<

▽　クレジット ( 敬称略 )

・　気まぐれな場所　( iso )
　　　http://kimagure.eucaly.net/

・　Cross Walker　( ティックル )
　　　http://cw7.sakura.ne.jp/index.html

>---------------------------------------------------------<