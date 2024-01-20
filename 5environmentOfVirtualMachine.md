## 5.仮想マシンの環境設定 ##
### 5-1.使用する仮想マシン（ここではAirGap）を選択し、「設定」アイコンをタップする ###
<img width="895" alt="１５：2024-01-20" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/ec85a7e2-02b9-4a27-a85f-9c06cadd17f4">

### 5-2.一般 ###
+ 「一般」→「高度」タブから**クリップボードの共有**と**ドラッグ＆ドロップ**を`「双方向」`に変更してOKをクリック
<img width="774" alt="１６：　　　 2024-01-04 202541" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/ed2b8e9f-452f-4206-b21b-9fb6daa01dd7">

### 5-3.システム ###
+ 「システム」→「マザーボード」タブの**フロッピー**の`チェックを外す`・**チップセット**を`ICH9に変更`してOKをクリック
<img width="772" alt="１７：　　　 2024-01-06 183847" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/b7aec409-438a-442c-87e4-f357799bcbbf">

### 5-4.共有フォルダの作成 ###
+ WindowsとUbuntu間の**共有フォルダ**(ここではShare)を作成する（ドキュメントフォルダなどの任意の場所）
> 共有フォルダを作成する際にフォルダの階層が深すぎると共有化できない場合があるので、階層を変えて作成してみてください。
<img width="880" alt="１８：　　　 2024-01-06 141528" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/0220b62c-f1f4-445c-a0b4-a723ef69c5e5">

### 5-5.仮想マシンから共有フォルダを指定選択する ###
+ 「フォルダーパス」に５-４で作成したフォルダを指定する
+ マウントポイントに`/media/share_win`を入力する
+ `自動マウント`にチェックする

![１９：　　　 2024-01-04 205659](https://github.com/SMAN8/Create-of-AirGap/assets/80440848/bce463bf-0e98-4b4e-8a80-eb6a5dd2d54f)

<img width="773" alt="２０：　　　 2024-01-04 204745" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/132c888d-2a5a-4f24-98ec-4126bb7f96d5">

