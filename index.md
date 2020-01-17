# 個人的なメモ（備忘録的なもの）

## ブロードキャストコマンド

Command + Shift + I

## パスワード付きzip

zip -e hoge.zip ファイル

## Slack のリマインダー

/remind 宛先 メッセージ on 日付 at 時間

## adb でスクショ

### スクショ

* adb shell screencap -p /sdcard/before_screen.png

### 録画

* adb shell screenrecord /sdcard/before.mp4

### 取得と削除

* adb pull /sdcard/before_screen.png
* adb shell rm /sdcard/before_screen.png
