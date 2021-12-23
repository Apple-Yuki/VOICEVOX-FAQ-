

## 動作環境・仕様に関する質問
### Q.動作環境を教えてください。Windows、 MacのOSに対応していますか？
Windows 10以上、macOS 11 Big Sur以降に対応しています。
またLinux OSにも対応しています。


## インストールに関する質問
### Q. インストールディレクトリはどこですか？
#### Windows版
デフォルトのインストール先は下記の場所です。  
`C:\Users\(ユーザー名)\AppData\Local\Programs\VOICEVOX`

#### Mac版
ダウンロードした「VOICEVOX」を手動でコピーした「アプリケーション」フォルダにあります。  
デフォルトのディレクトリは下記の場所です。  
`/Applications`
  
なお、システム管理者が制限を課してインストールしている場合は、以下のディレクトリに保存されることがあります。  
`/Users/(UserNames)/Applications`

### Q.Apple Silicon搭載のMacを使ってますがVOICEVOXは使えますか？
はい、使えます。なお、Rosettaをインストールする必要があります。  
過去にIntel 搭載モデルの Mac 用に開発された Appを使ったことがない方は、「VOICEVOX」をはじめて開く際に、Rosetta をインストールするかどうかを確認するメッセージが表示されます。  
Rosetta をいったんインストールしたら、Rosetta を必要とするほかの App でも使えるようになるので、再びインストールするよう案内されることはありません。
   
Apple Silicon搭載のMacとRosettaの詳しい情報はこちらのリソースをご覧ください。（Appleサポートページに飛びます）
- [Apple シリコン搭載の Mac コンピュータに関して](https://support.apple.com/ja-jp/HT211814)
- [Mac に Rosetta をインストールする必要がある場合](https://support.apple.com/ja-jp/HT211861)
- [技術情報:Appleシリコン搭載MacのRosetta 2](https://support.apple.com/ja-jp/guide/security/secebb113be1/web)

## 使い方に関する質問
### Q.オフラインのパソコンで利用できますか？
VOICEVOXはご利用のパソコンのシステム内部でWebサーバー機能を利用して動作します。  
ですので、クラウドサーバー等で処理してる訳ではなく、必ずインターネットに繋がってる必要はございません。


## 不具合・エラーに関する質問

### Q. エンジンの起動が失敗したというエラーが表示される

対応する GPU がないパソコンで GPU モードとして起動するとこのエラーが表示されます。設定 → エンジンから CPU モードを選んでください。
もしくは、起動に必要なファイルをウイルス対策ソフトが消去している場合があります。ウイルス対策ソフトをご確認ください。

#### Mac版
Mac版ではGPUモードに対応していないためGPUモードでは起動しません。

### Q. 音声が再生されない

エンジンの GPU モードで起動された場合は、一度 CPU モードをお試しください。（設定方法は１つ前で紹介しています。）  
また、ソフトウェアや PC を再起動することで再生されるようになることもあります。一度お試しください。


### Q. 長いテキストの音声が再生できない

GPU モードでよく発生する現象で、長い音声を生成するには多くのメモリが必要になり、メモリが溢れてエラーが発生します。よりメモリが多い GPU に乗り換えるか、CPU モードをご利用ください。

### Q. 「、」で区切った短い文節が読まれないことがある

現状の音声合成エンジンの仕様になります。前後の無音の長さを長くすると改善することがあるのでお試しください。

### Q. バージョンアップすると表示がおかしくなった

設定がなにか問題を起こしている可能性があります。一度ソフトウェアを終了して後述のパスにある設定ファイルを消去してもう一度起動してみてください。

#### Windows版

設定ファイルのパス：`C:\Users\(ユーザー名)\AppData\Roaming\voicevox`もしくは`voicevox-cpu`

#### Mac版
設定ファイルのパス①はVOICEVOX 側で能動的に使用している設定ファイルの保存先、設定ファイルのパス②はプログラムの構成とプロパティに関する情報を含む設定ファイルを管理している設定データとなっています。基本的に設定ファイルのパス①だけ削除すればいいですが、それでも改善しない場合、設定ファイルのパス②も削除してください。ログファイルは必要に応じて削除してください。

設定ファイルのパス①：`/Users/(UserName)/Library/Application\ Support/voicevox-cpu`

設定ファイルのパス②：`/Users/(UserName)/Library/Saved\ Application\ State/jp.hiroshiba.voicevox.savedState`

ログファイルのパス：`/Users/(UserName)/Library/Logs/voicevox-cpu `


## その他
### Q.電話音声など、音声のみを使いたい、仕事に使いたいのですが使用してもよいでしょうか？
VOICEVOXの通常ライセンスは個人のみに利用を仮定しております。  
電話音声など、音声のみを使いたい場合は各ライブラリーの音源利用規約をご覧ください。  
また、法人でのご利用、商用でご利用の場合は、各ライブラリー商用ライセンスを別途用意する必要がある可能性がございます。  
音源利用規約は以下の通りです。  
- [ずんだもん、四国めたん ](https://zunko.jp/con_ongen_kiyaku.html)
- [春日部つむぎ](https://tsukushinyoki10.wixsite.com/ktsumugiofficial/利用規約)
-  雨晴はう
-  [波音リツ](http://canon-voice.com/kiyaku.html)





### Q.どのような用途に使うことができますか？
各キャラクター毎の[キャラクター使用ガイドラインや具体的ケース] をご参照ください。こちらに具体的なケースの例やガイドラインがございます。


### Q.VOICEVOXの開発に協力したい。
不具合の修正など、誰でもVOICEVOXの開発や修正にもご参加頂けます。  
以下のコミュニティーをご確認ください。
- [VOICEVOX エディター](https://github.com/Hiroshiba/voicevox)
- [VOICEVOX エンジン](https://github.com/Hiroshiba/voicevox_engine)
- [VOICEVOX コア](https://github.com/Hiroshiba/voicevox_core)

### Q.問い合わせ先を教えてください。
ご感想・ご要望は、ぜひ Twitter にてハッシュタグ `#VOICEVOX` を付けてツイートしてください。

うまく動かない場合や不具合を見つけられた方は以下の内容を添えてハッシュタグ `#VOICEVOX` を付けてツイートしていただくか、  VOICEVOX公式（[@voicevox_pj](https://twitter.com/voicevox_pj)）までご報告ください。その他何かご質問があれば「よくあるご質問 （FAQ）」をご覧いただき、解決ない場合、[@hiho_karuta](https://twitter.com/hiho_karuta)までお問い合わせください。
