# Keyboard Quantizer

## About

Keyboard Quantizeの自分用ファームウェア

以下に対応

* 既定のレイヤーの際に、カーソル移動をスクロールに変更。

やりたいこと

* RelaconのメディアキーをRemapで変更できるようにする。

## 参照

[Keyboard Quantizer をマウスに使う | Kei's Portfolio](https://aficionerds.com/blog/20210728_mouse_quantizer/)

[『Keyboard Quantizer』について語るよ！ - 自作キーボード温泉街の歩き方](https://salicylic-acid3.hatenablog.com/entry/keyboard-quantizer-review)

## キーボード情報

<https://sekigon-gonnoc.github.io/Keyboard-Quantizer-B-Build-Guide/>

## ビルド方法

1. [ファームウェアのビルドと書き込み](https://sekigon-gonnoc.github.io/Keyboard-Quantizer-B-Build-Guide/build_firmware/)に従ってビルド環境を構築
2. <qmk\_firmware>/keyboardsにkeyboard\_quantizerという名前で本ディレクトリへのシンボリックリンクを貼る
3. <qmk\_firmware>下で、`make keyboard_quantizer/kqb:default:uf2`

## 覚書

2023/08/19現在、macOSのqmkだとmake時に以下エラーが出るため、
仮想ubuntuにて実行

```txt
argument {config,clone,console,env,setup,c2json,chibios-confmigrate,clean,compile}: conflicting subparser: console
```
