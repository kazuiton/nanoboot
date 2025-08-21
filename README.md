# NanoBoot
これは[**shimboot**](https://github.com/ading2210/shimboot)をカスタマイズしたものです。debianの起動に関するファイルを削除し、制限解除に特化させたものです。debianのデータがない分、容量は非常に小さく抑えることができました。使う前に起動させたいchromeosのバージョンによって、以下の手順を踏む必要があります。
## 使い方
### ver125~135の場合
1. nanobootを起動させてください。
2. **s ) enter a shell**という項目からshimのshellを起動させます。
3. ```135```を実行し、nanobootを再起動させます。
4. あとはroot-aまたはroot-bからchromeosを起動させましょう。
### ver136以上の場合
1. nanobootを起動させてください。
2. **s ) enter a shell**という項目からshimのshellを起動させます。
3. ```136```を実行し、nanobootを再起動させます。
4. あとはroot-aまたはroot-bからchromeosを起動させましょう。

詳しい手順は[かずいとんブログ](https://blog.kazuiton.com/2025/08/17/%e7%99%bb%e9%8c%b2%e3%81%95%e3%82%8c%e3%81%a6%e3%81%84%e3%82%8bchromebook%e3%81%a7%e3%83%9d%e3%83%aa%e3%82%b7%e3%83%bc%e8%a7%a3%e9%99%a4%e3%81%99%e3%82%8b%e6%96%b9%e6%b3%95%ef%bc%88nanoboot%ef%bc%89/)で解説しています。
## 構築方法
1. 自分のボードにあったRMA shimを[dl.kazuiton.com](https://dl.kazuiton.com/chromeos/rawshim)からダウンロードします。
2. ```git clone https://github.com/kazuiton/nanoboot&&cd nanoboot&&mkdir -p root```を実行します。
3. ```sudo ./build.sh example.bin path_to_shim root```を実行します。作成されたイメージはexample.binとして出力されます。
## 参考であり大本
[ading2210`s shimboot](https://github.com/ading2210/shimboot)
