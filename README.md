# NanoBoot
これは[**shimboot**](/https://github.com/ading2210/shimboot)をカスタマイズしたものです。debianの起動に関するファイルを削除し、制限解除に特化させたものです。debianのデータがない分、容量は非常に小さく抑えることができました。使う前に起動させたいchromeosのバージョンによって、以下の手順を踏む必要があります。
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
## 構築方法
1. 自分のボードにあったRMA shimを[dl.kazuiton.com](https://dl.kazuiton.com/chromeos/rawshim)からダウンロードします。
2. ```git clone https://github.com/kazuiton/nanoboot&&cd nanoboot&&mkdir -p root```を実行します。
3. ```sudo ./build.sh example.bin path_to_shim root```を実行します。作成されたイメージはexample.binとして出力されます。
## 参考であり大本
[ading2210`s shimboot](https://github.com/ading2210/shimboot)
