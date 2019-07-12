# micro:bit 程式體驗

## 使用前準備

### 將 micro:bit 連接到個人電腦

將 micro:bit 以 micro USB 纜線連接到個人電腦上的 USB 連接埠即可。

### 啟動程式設計軟體

點擊下列連結，進入 micro:bit 的程式編輯介面

https://makecode.microbit.org/

並按下新增專案(New Project)，便可以開始進程式的編寫

為了達到最佳體驗，請務必使用 Google Chrome 瀏覽器

詳細的連接與使用步驟，可以參考 micro:bit 官網的說明

https://microbit.org/guide/quick/

### 如何將程式碼存檔

## Project: 瘋狂計步器

```blocks
input.onGesture(Gesture.Shake, function () {
    step += 1
})
input.onButtonPressed(Button.AB, function () {
    step = 0
    basic.showIcon(IconNames.Heart)
    basic.pause(1000)
})
let step = 0
step = 0
basic.showIcon(IconNames.Heart)
basic.pause(1000)
basic.forever(function () {
    basic.showNumber(step)
})
```
