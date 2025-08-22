# NanoBoot
これは[**shimboot**](https://github.com/ading2210/shimboot)をカスタマイズしたものです。debianの起動に関するファイルを削除し、制限解除に特化させたものです。debianのデータがない分、容量は非常に小さく抑えることができました。使う前に起動させたいchromeosのバージョンによって、以下の手順を踏む必要があります。
## 構築済みファイル
[kazuiton's file host](https://dl.kazuiton.com/chromeos/prebuild/nanoboot)
## 使い方
1. nanobootを使い、chromeosのaまたはbパーティションからchromeosを起動させます。
2. [ctrl+alt+f2]キーを押した後、"root"と入力しrootユーザーでshellも起動させます。
3. v124以下の方は'''124'''と、v125~135までの方は'''135'''と、V136以上の方は'''136'''と黒い画面に打ち込んでください。
4. [ctrl+alt+f1]でchromeosのguiに戻りセットアップをしていけば完了です！

詳しい手順は[かずいとんブログ](https://blog.kazuiton.com/2025/08/17/%e7%99%bb%e9%8c%b2%e3%81%95%e3%82%8c%e3%81%a6%e3%81%84%e3%82%8bchromebook%e3%81%a7%e3%83%9d%e3%83%aa%e3%82%b7%e3%83%bc%e8%a7%a3%e9%99%a4%e3%81%99%e3%82%8b%e6%96%b9%e6%b3%95%ef%bc%88nanoboot%ef%bc%89/)で解説しています。
## 構築方法
1. 自分のボードにあったRMA shimを[dl.kazuiton.com](https://dl.kazuiton.com/chromeos/rawshim)からダウンロードします。
2. ```git clone https://github.com/kazuiton/nanoboot&&cd nanoboot&&mkdir -p root```を実行します。
3. ```sudo ./build.sh example.bin path_to_shim root```を実行します。作成されたイメージはexample.binとして出力されます。
## 参考であり大本
[ading2210`s shimboot](https://github.com/ading2210/shimboot)
