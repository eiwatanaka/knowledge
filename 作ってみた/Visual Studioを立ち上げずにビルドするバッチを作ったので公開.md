## 1. はじめに

「Gitに最新ソースプッシュしたから動作確認しておくれーーー」ってなったとき、
今使っているPCのスペックがイマイチで、Visual Studioの起動にとても時間がかかっていました。
いちいち起動してビルドするのが面倒だったので、MSBuildを使って(なるべく)汎用的に使えそうなバッチを作ってみました。

## 2. GitHub

[sln_builder](https://github.com/i-tanaka730/sln_builder)

## 3. ユーザー変数についての説明

```
rem MSBuildのパス
set MSBUILD_PATH=C:\Windows\Microsoft.NET\Framework\v4.0.30319\MSBuild.exe
```

MSBuildのパスを設定します。
Windows7以降は標準でインストールされているようですが、古い場合等は以下からインストールできます。
https://www.microsoft.com/ja-JP/download/details.aspx?id=48159

```
rem ソリューションファイルのパス
set SOLUTION_FILE=C:\xxxxx\xxxxx.sln
```

ソリューションファイルのパスを設定します。


```
rem ビルド構成 (debug / release)
set BUILD_CONFIG=debug

```

ビルド構成を設定します。
デバッグビルドの場合は「debug」、リリースビルドの場合は「release」を設定してください。


```
rem ビルド種類 (build / rebuild)
set BUILD_TYPE=build
```

ビルド種類を設定します。
ビルドの場合は「build」、リビルドの場合は「rebuild」を設定してください。

```
rem 最新ソース取得有無 (true / false)
set PULL_SOURCE=false
```

最新ソースを取得するかどうかを設定します。
最新ソースを取得する場合は「true」、取得しない場合は「false」を設定してください。


```
rem ブランチのパス
set BRANCH_PATH=C:\xxxxx
```

最新ソースを取得するブランチのパスを設定します。
最新ソースを取得する場合は設定必須、取得しない場合は設定不要です。


```
rem ブランチの名前
set BRANCH_NAME=xxxxx
```

最新ソースを取得するブランチ名を設定します。
最新ソースを取得する場合は設定必須、取得しない場合は設定不要です。




