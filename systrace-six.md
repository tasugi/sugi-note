# Android の Systrace を実行すると "ImportError: No module named six" と表示される

Android 開発ツールである Systrace を実行しようとしたら、
`ImportError: No module named six`
と表示され、Systrace を実行できないことがありました。

**six** という Python のモジュールが不足しているのが原因のようです。

Python のパッケージマネージャである pip を使ってモジュールをインストールすれば、
エラーを解消できます。
```
$ pip install six
```

Ubuntu か Debian を使っているのであれば、
apt からもインストールすることができます。
```
$ apt install python-six
```
