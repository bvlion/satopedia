# 個人的なメモ（備忘録的なもの）

## ブロードキャストコマンド

Command + Shift + I

## パスワード付きzip

zip -e hoge.zip ファイル

## Slack のリマインダー

/remind 宛先 メッセージ on 日付 at 時間

## Git

### 削除

* `git branch -d`
* 未マージ `git branch -D`

https://qiita.com/hogeta_/items/33d2334c9b1919bd5120

### 特定のファイル

`git log -p /dir/target.file`

### 特定の行

`git log -L 70,80:/dir/target.file`

## adb でスクショ

### スクショ

* adb shell screencap -p /sdcard/before_screen.png

### 録画

* adb shell screenrecord /sdcard/before.mp4

### 取得と削除

* adb pull /sdcard/before_screen.png
* adb shell rm /sdcard/before_screen.png

## DebugView
https://firebase.google.com/docs/analytics/debugview?hl=ja

トラッキング開始
```
adb shell setprop debug.firebase.analytics.app package_name
```
トラッキング終了
```
adb shell setprop debug.firebase.analytics.app .none.
```

![参考](https://user-images.githubusercontent.com/24517539/77731856-17a68780-7047-11ea-82e8-fb0892f35ac4.png)

## 無線 adb

* USB 接続して `adb tcpip 5555` を実行（5555 でなくてもいい）
* adb connect <device-ip-address> （IP は設定のデバイス情報や Wi-Fi の設定などに記載されている。固定 IP がよさそう。）
* 切断は `adb disconnect`

## しばらくの間のバイブル

https://qiita.com/takahirom/items/3f012d46e15a1666fa33
