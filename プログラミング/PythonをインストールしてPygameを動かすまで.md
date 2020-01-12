## 1. はじめに

最近はPythonがQiitaタグランキングを独占。
超トレンドになっているのにも関わらず、~~プロジェクトで使う機会がなかった~~触れていなかったので、入門していきたいかと思います。

## 2. Pythonで作れるもの
Pythonはシンプルかつ高機能な言語であるため、様々なシステムで活用されています。
Pythonで作れるものは大きく分けると「WEBアプリ」「データ解析／分析ツール」「人工知能」になります。
また、Pythonで作られているシステムには以下のようなものがあります。

* WEBアプリ
 * YouTube
 * Instagram
 * Dropbox
 * Pinterest
* データ解析／分析ツール
 * Jupyter
 * graph-tool
 * Numpy
 * Pandas
 * Scipy
* 人工知能
  * Pepper

## 3. Pythonのインストール
では早速開発環境を作っていきましょう。今回の構築先はWindowsです。
Pythonのバージョンは3.6.5になります。(2018/06/23時点)
Pythonのインストールは以下から行います。
https://www.python.org/downloads/

①「Download Python 3.6.5」をクリックし、インストーラーをダウンロードします。
![1.png](https://qiita-image-store.s3.amazonaws.com/0/247638/a694899c-617c-a041-6ee3-c33783f798ac.png)

②自動で環境変数にパスを追加するため、「Add Python 3.6 to PATH」にチェックを入れ、「Install Now」をクリックします。
![2.png](https://qiita-image-store.s3.amazonaws.com/0/247638/2ee3a38f-769c-2146-f650-b0ba86eadf99.png)

③インストールが完了したら、「Close」をクリックしてダイアログを閉じます。
![3.png](https://qiita-image-store.s3.amazonaws.com/0/247638/c4fd6e9c-2795-2044-9d55-99b24f0974af.png)

④コマンドプロンプトを起動し、「python --version」と打ちます。バージョンが表示されれば成功です。
![4.png](https://qiita-image-store.s3.amazonaws.com/0/247638/23e38881-8c32-aa0a-2e56-59d627ed89f1.png)

## 4. Pygameのインストール
続いてはPygameのインストールを行います。

①コマンドプロンプトを起動し、「python -m pip install pygame」と打ちます。
![g1.png](https://qiita-image-store.s3.amazonaws.com/0/247638/0c0b4d4d-8408-22a8-b9cf-5c06ba2e123b.png)

②「python」コマンドを打ったあと、「import pygame」と入力し、エラーが表示されなければ成功です。
![g2.png](https://qiita-image-store.s3.amazonaws.com/0/247638/bb30d6ef-9553-6d32-8636-0bed4f884fd7.png)

## 5. Pygameを動かしてみる
Pygameのインストールが成功すると、以下にPygameフォルダができあがると思います。
"C:\(ユーザフォルダ)\AppData\Local\Programs\Python\Python36-32\Lib\site-packages"
たくさんのサンプルゲームがインストールされますので、以下のサイトを参考にしてみて下さい。
http://westplain.sakuraweb.com/translate/pygame/Examples.cgi

今回はインベーダーゲームをしてみましょう。
①コマンドプロンプトで、「python -m pygame.examples.aliens」と打ちます。
![1.png](https://qiita-image-store.s3.amazonaws.com/0/247638/41ed1080-8deb-cb02-1387-e2b678f1b7a9.png)

②インベーダーゲーム起動します！
![2.png](https://qiita-image-store.s3.amazonaws.com/0/247638/c1115cf9-95c0-9d75-f37d-90e835d3cc75.png)

## 6. PythonのIDE(おまけ)
PythonのIDEは以下のようなものがあります。
~~中でもPyCharmがイケイケらしいです。~~
個人的にはやはりVisual Studio派でした(^^;)

|名前   |URL|
|---|---|
| PyCharm| https://www.jetbrains.com/pycharm/|
| IDLE| (Pythonに付属)|
| Eclipse	| https://www.eclipse.org/|
| PyScripter	| https://sourceforge.net/projects/pyscripter/|
| Wing	| https://wingware.com/|
| Visual Studio Code| https://www.microsoft.com/ja-jp/dev/products/code-vs.aspx|
| Visual Studio Community| https://www.microsoft.com/ja-jp/dev/products/community.aspx|
