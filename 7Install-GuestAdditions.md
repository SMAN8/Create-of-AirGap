## 7.Guest Additionsのインストール ##
+ アプリ一覧からターミナル(端末)を起動し以下コマンドを手動入力する。

```
sudo apt update -y
sudo apt upgrade -y
sudo apt install gcc make perl -y
```

> まだコピーアンドペーストが利用できない為、タイプミスに留意して下さい。

### 7-1.ホストメイン画面上部の`デバイス`タブから`Guest Additions CDイメージの挿入…`をタップします。 ###

<img width="519" alt="４７：　　　 2024-01-05 190705" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/40550769-f022-4c8e-a10c-5b98e5a0dd9d">

### 7-2.以下のメッセージが表示されたら`実行(R)`をクリックした後、パスワードを入力し、`認証ボタン`をタップします。

<img width="518" alt="４８：　　　 2024-01-05 191029" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/15b78338-b7f9-4a5f-9aad-d7b80be207fc">

### 7-3.下の画像内の赤いラインのように処理完了のメッセージが表示されましたら、`Enter`キーをタップします。

<img width="518" alt="４９：　　　 2024-01-05 191712" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/bdf95e54-5a58-45a5-9cb8-1e924a83ee79">

### 7-4.ターミナル(端末)を起動しユーザーをグループ化するコマンドを実行 ###

> 左上のアクティビティをタップします。そして検索窓にterminalの`t`と入れると下の画像のように端末が表示されます。

<img width="519" alt="５０：　　　 2024-01-05 201746" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/99d7f0a0-6861-4a0d-805a-c2246c47df6b">

> 端末をタップし、起動させユーザーをグループ化するコマンドを実行

```
sudo adduser $USER vboxsf
```

<img width="520" alt="５１：　　　 2024-01-05 202410" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/8d75aba5-f011-46dc-8bcb-b034403c9a9b">

> 下の画像のようにユーザーがグループ化された事を端末で確認できます

<img width="518" alt="５２：　　　 2024-01-05 202644" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/6c56cfba-237a-4558-8a05-db9aeb1620bd">

### 7-5.フォルダに`share_win`が表示されていれば、5-5.の「共有フォルダ」で設定したローカルPCのフォルダと同期します。 ###

<img width="519" alt="５３：　　　 2024-01-05 203211" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/9d90b7c4-3288-455b-9530-4d03b1c8a897">

### 7-6.コピー＆ペーストできるか`ホストPC`でテキスト文字をコピーして`ゲストOS`の端末で右クリックして貼り付けしてみる。
> メモ帳にコピー用として`aiueo`と入力し、`Ctrl + A`で全選択→`Ctrl + C`でコピーする

<img width="649" alt="５４：　　　 2024-01-06 185300" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/658ef1ca-69a2-40c3-b12d-b2c18c5fa7c8">

+ 仮想マシンのUbuntuOS内の端末に`Ctrl + V`でペーストする。ペーストできたら、OKです。

+ もし、コピー＆ペーストできなかった場合は、下の対処方法を行ってみてください。

<img width="398" alt="５５：　　　 2024-01-06 185826" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/0fa41760-1f2e-4c25-b830-746925204e5c">

### コピー＆ペーストが出来なかった場合の対処方法 ###
+ 端末を開き、右上の`ハンバーガーボタン`をタップし、`設定(P)`をタップする

<img width="401" alt="５６：　　　 2024-01-06 185107" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/fdd16f50-4688-4c95-b9ad-e757c30b3633">

+ `ショートカットタブ`をタップし、編集の中の`コピーと貼り付け`のショートカットを確認。
+ コピーのショートカットが、`Shift + Ctrl + C`、貼り付けのショートカットが`Shift + Ctrl + V`になっている場合があります。ローカルPCのショートカットと一緒に変更しておくと、楽なので、それぞれコピーと貼り付けを`Ctrl + C`と`Ctrl + V`に変更しておきます。
+ それぞれのショートカットキーを変更したら、端末でコピー＆ペーストを試してみてください。

<img width="476" alt="５７：　　　 2024-01-06 191013" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/3038e42f-768c-439c-9626-c5c2c9703d96">

### 7-7.表示→ゲストOSの画面を自動リサイズにチェックが入っている事を確認します。
+ チェックが入っていなければ、チェックを入れて下さい。

<img width="475" alt="５８：　　　 2024-01-06 192216" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/1f60c434-17a5-4e10-8dae-cd0ddb488f8e">

+ 上記手順を行っても、「共有フォルダが表示されない」「共有フォルダ化されていない」場合は、一度VBox_GAs_7.0.12をアンマンウントしてから再度挿入し、再起動すると共有フォルダは完了します。


