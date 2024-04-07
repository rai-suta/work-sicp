# work-sicp
「計算機プログラムの構造と解釈」
https://sicp.iijlab.net/

## 環境構築 - Debian
参考：https://practical-scheme.net/gauche/download-j.html

gaucheのインストール
```
$ sudo apt install build-essential
$ curl https://raw.githubusercontent.com/shirok/get-gauche/master/get-gauche.sh -o get-gauche.sh
$ bash ./get-gauche.sh
...
################################################################
#  Gauche installed under /usr/local/{bin,lib,share}
################################################################
```

参考：https://practical-scheme.net/gauche/man/gauche-refj/GauchewoQi-Dong-suru.html

バージョンの確認
```
$ gosh -V
Gauche scheme shell, version 0.9.14 [utf-8,pthreads], x86_64-pc-linux-gnu
(version "0.9.14")
(command "gosh")
(scheme.id gauche)
(languages scheme r5rs r7rs)
(encodings utf-8)
(website "https://practical-scheme.net/gauche")
(build.platform "x86_64-pc-linux-gnu")
(build.configure "--prefix=/usr/local")
(scheme.path "/usr/local/share/gauche-0.98/site/lib" "/usr/local/share/gauche-0.98/0.9.14/lib")
(threads pthreads)
(gauche.net.tls)
```

gosh の起動と終了
```
$ gosh
gosh$ (print "Hello gosh!")
Hello gosh!
#<undef>
gosh$ (+ 1 2)
3
gosh$ (exit)
```
