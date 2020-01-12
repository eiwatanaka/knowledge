## 1. はじめに

スマホアプリを開発するにあたり、**React Native**が流行ってきているようですね。
React Nativeに触れる前に、まず<font color="red">**React**</font>について勉強しとかないといかんなということで、記事にまとめておきたいと思います。


## 2. Reactとは

開発元はFacebookで、一言でいうと<font color="red">**UI部品を作るためのjavaScriptライブラリ**</font>になります。
Facebook、Instagram、GitHub ATOM、Twitterモバイル等で使用されています。

## 3. Reactの特徴

#### 3-1. Just the UI

フレームワークでなく、あくまでUIを構築するためのライブラリになります。MVCでいうVのみ機能を提供します。
ライブラリに属するため、Angular.jsやBackbone.jsと<font color="red">**一緒に使用することが可能**</font>です。

#### 3-2. Virtual DOM

実際のDOMと対となる構造体を用意し、その構造体に対して処理を行います。
その結果生まれた差分だけを実際のDOMに反映することで、<font color="red">**UI表現の高速化**</font>を実現しています。

#### 3-3. Data flow

データの変更に応じてUIの変更が行われる、単方向データバインディングの仕組みが利用されています。
そのため、コードの複雑性を避け、<font color="red">**シンプルな設計が可能**</font>となります。
(ちなみにVue.jsは双方向データバインディング)

## 4. Reactで作られたWebアプリ

＜[Made with React](https://madewithreact.com/)＞

上記のサイトで、React(もしくはReact Native)で作られたWebアプリがギャラリー形式で掲載されています。Reactを使うとこんなものが作れるんだーとイメージできるかもです。

## 5. Reactの環境構築

#### 5-1. Node.jsのインストール

Reactの環境構築には、Node.js(Ver4以上)がインストールされている必要があります。
Node.jsのインストール方法については以下を参照ください。

- [Node.jsを学ぶ中で必ず押さえておきたいこと](https://qiita.com/i-tanaka730/items/79e8e2c3ceb2bde51436)

#### 5-2. Reactのインストール

以下のコマンドを実行するだけです。

```
npm install -g create-react-app
```

## 6. アプリの作成とサーバーの起動確認

#### 6-1. アプリの作成

以下のコマンドを実行します。

```
create-react-app test-app (作成したいフォルダ名)
```
すると以下のような構成でフォルダができます。

![test-app.PNG](https://qiita-image-store.s3.amazonaws.com/0/247638/65c55cc0-995b-e2cc-61e2-1298d44d3021.png)

#### 6-2. サーバーの起動確認
作成したフォルダへ移動し、サーバーを起動します。

```
cd test-app  // 移動して
npm start    // 起動！
```
ブラウザにて http://localhost:3000/ にアクセスします。
以下のような画面が表示されればOKです。

![起動.PNG](https://qiita-image-store.s3.amazonaws.com/0/247638/d97e5cd6-7d48-9394-0136-2a97f7683e1f.png)

## 7. IDE

ReactのIDEは<font color="red">**Visual Studio Code**</font>がおススメです。
Visual Studio Codeでは以下のようにしてデバッグを行うことができます。

#### 7-1. Debugger for Chromeをインストール

Visual Studio Codeの拡張機能メニューから、**Debugger for Chrome**をインストールします。

![vdcode.png](https://qiita-image-store.s3.amazonaws.com/0/247638/86cb3915-f25a-05a5-01ad-77e89ea223f6.png)

#### 7-2. launch.jsonの設定

**launch.json**を開き、以下のように設定します。
(url、webRootは環境に合わせて書き換えてください。)

![設定.png](https://qiita-image-store.s3.amazonaws.com/0/247638/7b53bf7e-7663-64e0-8f87-1037af86a907.png)

#### 7-3. デバッグする

サーバーが起動していなければ起動してください。
その後以下のボタンからデバッグが行えます。(メニューから、**デバッグ** ⇒ **デバッグの開始**でもOK)
もちろんブレークポイントもはれます。
てかデバッグ実行と同時に起動することもできるのか？？？

![デバッグ.png](https://qiita-image-store.s3.amazonaws.com/0/247638/c999d760-81ed-3936-67db-2e7110594691.png)


#### Reactide

React専用のIDE＜[Reactide](http://reactide.io/)＞も触ってみましたが、開発中であるためか、New Projectした時点で応答なしになりました。。。正式にリリースされるまでは使用は控えた方がいいかもです。
何か情報を持っている方は展開頂けると嬉しいです。

## 8. おわりに

まだ構文はなかなか慣れれずにいます^^;

- [Node.jsを学ぶ中で必ず押さえておきたいこと](https://qiita.com/i-tanaka730/items/79e8e2c3ceb2bde51436)

で勉強したことと合わせて、Node.js + Reactなアプリを作ってみたいかと思います。
