## 1. はじめに

以下雑誌の要約。

- 題名：日経SYSTEMS 2019/1号


## 2. トラブルの火消し術

### ～要約～

#### 2-1. この章について
火を噴き始めたプロジェクトの被害は甚大である。スケジュールは遅れ、メンバーは疲労し、ユーザーとベンダーの仲は険悪になる。プロジェクトの火種やプロジェクトをどう立て直すのかついて以下にまとめる。

#### 2-2. プロジェクトの火種が増えている
システム開発プロジェクトのトラブルの火種は増えてきている。最近の要因としては以下のようなものが挙げられる。

##### 2-2-1. アジャイル開発の増加
- アジャイル型では、進捗管理やレビューなど、従来のウォーターフォール型とは異なるマネジメントスキルが必要になる。また、ベンダーに対してシステムを発注するユーザー企業の期待値は高くなることが多い。
- アジャイル型に「安い」「早い」というイメージを持つユーザーも少なくない。本当にアジャイルのアプローチが正しいかどうかを判断すべき。

##### 2-2-3. スキル不足
- プロジェクトに関わるメンバーのスキル不足は、トラブルに直結する。プログラミングは早いが、テストでバグが噴出するプログラマーが少なくない。プログラマーが自分の裁量でテストしているだけで、テストシナリオがきちんと書けないため。

#### 2-3. 求められる火消しのワザ
プロジェクトに火がつく要因は様々だが、例えば以下のような対策がある。

##### 2-3-1. 最大公約数で課題を捉える
- 問題解決にあたって、**最大公約数で課題を捉える**というアプローチがある。トラブルに対して、手当たり次第に対策を打つのではなく、**最も効果が得られる対策**に絞り込むとよい。
- 例えば「業務知識不足」「技術スキル不足」「大型プロジェクト経験が少ない」「コミュニケーションが弱い」という課題があったとすると、**多くのメンバーに共通する問題はどれか**を特定し、その問題に対してまずは解決を図る。

##### 2-3-2. 打ち合わせをの形式を変える
- 打ち合わせ等において、ささいなことでユーザーとの関係が険悪になってしまうことがある。このような場合にできる対策が、ユーザー1人1人と打ち合わせを実施する方法である。1人1人と打ち合わせをすることで、**本当に必要な機能**や**本音**を引き出すことができる。

#### 2-4. 炎上は未然に防げる
プロジェクトの炎上を避けるには、リスクを洗い出し、事前に対策を打つ必要がある。プロジェクトの進捗などからリスクを嗅ぎ取り、先手を打てればトラブルは未然に防げる。トラブルを未然に防ぐには、以下のようなことが重要となる。

##### 2-4-1. ドキュメントを残す
- トラブルを引き起こす大きな火種は、ユーザーとベンダーとの意見の食い違い。**合意事項リスト**や**背景サマリー**を作成するなどして対策を打つ。何をどこまで作るかユーザーと開発チームできっちりと合意する。場合によってはチャット履歴やメール履歴も引き継ぎ資料として残すべき。これにより、プロジェクトメンバーの交代にも備えられる。

##### 2-4-2. スキルアップを図る
- スキルはフロントからバックエンドまで理解しているのが望ましい。**トラブル発生時の問題切り分け**のためにも幅広いスキルが必要になる。
- 最新スキルを学ぶことも重要。開発やテストの自動化で開発効率を高めるためには、最新ツールの使いこなし等がかかせない。個人のスキルだけでなく、**開発チーム全体でスキルが足りているかどうか**も事前に押さえておくとよい。


### ～感想～
炎上とまではいかなくとも、プロジェクトにおいて問題が発生することは多々ある。「問題解決」や「問題を防ぐ」ということに対して、メンバー個のスキル(技術/マネジメントetc...)が非常に重要だと感じた。(本田圭佑っぽいが)個のスキルは確実にチームの全体の力となる。幅広く知識を吸収しておくことで、必ずどこかで成果に繋がる！選択肢も増える！


## 3. Webアプリを変える新仕様　PWA丸わかり

### ～要約～

#### 3-1. この章について
WebシステムやWebアプリケーションは、新仕様の**PWA(Progressive Web Apps)**で進化する。
PWAとは**Webアプリでネイティブアプリのような優れた体験を提供すること、またはそれを実現するための技術仕様**を指す。
これまでのWebアプリでは、実現しにくかったWeb閲覧の高速化やオフラインでの利用などが可能になり、より業務利用での活用範囲が広がる。


#### 3-2. PWAで作るメリット

- システムをネイティブアプリで作るか、Webアプリで作るかについて、開発や保守の観点で以下のような違いがある。

|項目          |ネイティブアプリ                            |従来のWebアプリ                               |
|:-------------|--------------------------------------------|----------------------------------------------|
|動作速度      |ハードウェアの性能をフルに活用できるので高速|ブラウザを介するので遅い                      |
|デバイスの機能|端末に搭載される全ての機能を使える          |ブラウザから利用できる機能に限られる          |
|オフライン対応|オフラインでも仕様可能                      |インターネットに接続していなければ利用できない|
|配布          |アプリストアを経由してダウンロードが必要    |ブラウザで特定のURLにアクセスするだけで使える |
|開発スキル    |対応OSごとに専門知識が必要                  |Web関連の共通知識で開発可能                   |

- 2018年初頭から普及し始めたPWAによって、この状況が変わってきた。PWAは**Webアプリでありながらオフライン環境でも動作する**。またプッシュ通知を受け取ったりする仕様も、ブラウザへの機能追加が進むにつれて使えるようになってきた。
- PWAを採用すれば、**標準としてのWebの利点はそのままに、ネイティブアプリに匹敵する機能性と使い勝手を実現できる**ことになる。さらに各デバイスで共通のコードで開発できるので、**開発工数**の削減にもつながる。
- PWAの適用事例は、国内の企業でも増え続けている。リクルート住まいカンパニーのSUUMOは、早くからWebサイトのPWA化に取り組んでいる。成果として、PWA化でページの読み込み時間を75％削減した。ほかに、日本経済新聞社が日経電子版をPWA化して表示を高速化した事例もある。


#### 3-3. PWAを支える技術

PWAを構成する技術としては、主に以下のようなものがある。

##### 3-3-1. 見栄えに関する設定ファイルの「App Manifest」

- App Manifestは、**PWA対応アプリのアイコン名やアイコン画像、起動時の背景色などを決める設定ファイル**となる。
- 実体はJSON形式で記述する。PWA対応アプリを作成する際は、App Manifestに設定項目を記載し、それをWebサーバー上に配置する。このファイルをWebブラウザーがHTMLファイルなどと一緒に読み込むことで、PWAアプリの設定が可能になる。
- App Manifestには主に以下のような項目を記述する。

|キー            |値の概要                                    |
|:---------------|--------------------------------------------|
|background_color|起動した際のスプラッシュスクリーンの背景色を指定する。|
|display         |起動方法を指定する。<br>スマホアプリのように単独で起動する「standalone」<br>ステータスバーを表示しない「fullscreen」<br>ブラウザを使った表示の「brrowser」<br>などがある。
|icons           |ホーム画面に配置するアイコンを指定する。|
|name            |アプリの名前を指定する。|
|short_name      |アプリの短い名前を指定する。表示領域が狭いときに利用する。|
|start_url       |起動時に読み込むURLを指定する。|
|theme_color     |ツールバーの色を指定する。|

##### 3-3-2. オフラインを実現するキャッシュ技術の「Service Worker」

- Service Workerは、**Webアプリをオフライン対応させたり、プッシュ通知を可能にしたりする処理を記述したプログラム**。
- JavaScriptで記載されており、App Manifestと同様にWebサーバーに配置する。PWAに対応したブラウザは、App ManifestやService Workerを読み込み、Service WorkerのJavaScriptプログラムがあれば、PWA対応アプリとして動かす。
- **コンテンツのキャッシュ**はService Workerによって実現する。ここでいうコンテンツとは、HTML/CSS/JavaScript/画像ファイル、Web APIのレスポンス内容などである。これらを**アクセス時にキャッシュしておき、2回目以降のアクセス時やオフライン時にはキャッシュからデータを返す**。これにより、パフォーマンスの向上やオフライン時の利用が可能になる。
- データの保存には、Webブラウザーに内蔵されている4つのキャッシュ「Cookie」「localStorage」「Cache API」「IndexedDB」のうちいずれかを利用する。Service Workerでは、Cache APIやIndexedDBが使われることが多い。現時点では、Android 5以降、iOS 11.3以降でService Workerを利用できる。(ただし、iOSでは機能に制限があり、ホーム画面にアイコンを配置できない。)

##### 3-3-3. スマホ専用の「プッシュ通知」がブラウザで実現可能に

- PWA対応アプリでは、プッシュ通知も可能。ユーザー自身が取得操作をせずに、イベントに応じて画面上に通知を表示できる。
- プッシュ通知はこれまで、スマホアプリ専用の機能だった。プッシュ通知を実現するのに、スマホアプリを開発するといったニーズがあったほど。それがPWAの登場で、**Webアプリでもプッシュ通知を送受信できるようになった**。
- 現時点ではPWAのWebプッシュ通知はスマホやタブレットではAndroidだけがサポートしている。残念ながらiOSではWebプッシュ通知を表示できない。デスクトップPC向けブラウザーのGoogle ChromeやFirefox、Edgeでは標準仕様として対応している。Safariでは、macOSの独自機能を使ってWebプッシュ通知に対応しなければならない。
- Webプッシュ通知の実現方法は、大きく「Notifications API」「Push API/VAPID」「macOS Safari独自のWebプッシュ通知」「Google Chrome独自のWebプッシュ通知」の4つがある。

### ～感想～

スマホを使う機会、時間は爆発的に増えてきているので、こういった技術は人間にとってとても嬉しい。
ググってみると、チュートリアルとかも結構あるので体験してみようと思う。そして相変わらずJavaScriptの技術はすごい。


## 4. [テスト設計] 範囲、観点、条件を検討 主要5項目をテストケースに

### ～要約～

#### 4-1. この章について
テスト計画を基に、テストで確認したいことを具体化してテストケースを作成するプロセスがテスト設計である。ただしいきなりテストケースは作れない。指針もなく作業を始めてしまうと、担当者ごとの認識や知識の違いがそのまま成果物のばらつきに繋がってしまう。事前にテストケース作成方法を検討し、テストの範囲と観点、条件をテストタイプごとに決めていく。テスト設計のポイントを以下にまとめる。

#### 4-2. テストケース作成方針の検討
テストケース作成方針では、**テスト範囲、テスト観点、テスト条件**を決めていく。

##### 4-2-1. テスト範囲
- テスト範囲の検討では、**テストするところ**と**テストしないところ**を切り分ける。
- テスト計画で検討したテスト対象は、業務や機能といった大きな粒度になっている。テストケース作成方針では、より細かい単位まで分解して検討する。ECサイトを例にとると、「商品管理機能」は「商品登録機能」「商品参照機能」「商品更新機能」「商品削除機能」などに分解して検討する。

##### 4-2-2. テスト観点
- テスト観点の検討では、テストで確認すべきことを決める。テスト範囲内にあるテストの対象ごとに、**何を確認すべきか**を決めていく。

##### 4-2-3. テスト条件
- テスト条件の検討では、テスト観点ごとにテスト条件を整える。ここでいうテスト条件とは、**テスト対象の状態や与えるデータ、操作方法などのバリエーション**のことである。
- スケジュールやコストに制約があるため、あらゆるバリエーションのテストは非現実的となる。**テスト計画で決めた優先順位**を踏まえて網羅する基準を決める。

#### 4-3. テストケースの作成方法
テストケースの作成方針が固まったら、いよいよテストケースを作成する。テストケースとは、**テストの具体的な作業手順や期待結果をまとめたドキュメント**となる。
テスト計画、テストケース作成方針で決めた通りにテストを実行できるようにするためには、以下の5要素が書かれていることが望ましい。

##### 4-3-1. テスト対象
- テスト対象には、**テストすべき対象(システムのどの部分を確認するのか)**を書く。
- テストケース作成方針で決めたテスト範囲の表現は、テストケースでそのまま使うには粒度が大きすぎる場合が多い。そこで、**テスト範囲を分割してテストケースに記載**する。例えば、テストケース作成方針でテスト範囲が画面単位だったとしたら、「画面名」「エリア名」「項目名」という単位に分割する。分割する単位はテストケース作成前に決めておくことが望ましい。

##### 4-3-2. テスト観点
- テスト観点には、**テストで確認したいこと**を書く。
- テスト観点はテストケース作成方針で検討した内容が基となる。
- テスト観点では**一読してそのテストケースの目的・意図が把握できる**ようにする。こうすると、テスト対象とテスト観点を見れば、大まかなテスト内容を把握でき、確認したい内容がテスト実行者やレビュアに伝わりやすくなる。

##### 4-3-3. テスト条件
- テスト条件には、**テスト結果に影響を及ぼすだろう要素**を書く。
- 例えば**システムの状態や入力データ、操作のバリエーション**がテスト条件となる。これらの要素について、取りえる値や状態を検討する。
- 同じテスト対象・テスト観点に対して複数のテスト条件が存在する場合は、テスト条件のパターン表を作ると分かりやすい。

##### 4-3-4. テスト手順
- テスト手順には、**テストで確認すべき結果が出力されるまでの作業手順**を書く。
- **テスト実施者が誤りなく操作できる**ようにする。画面名や項目名などは、仕様書に定義されているものをそのまま使用すると誤解が少ない。

##### 4-3-5. 期待値
- 期待値には、**どのような結果になっていれば合格か、期待される結果**を書く。
- **読み手にとって解釈が異ならないように注意**する。「○○項目に××と表示されていること」といった形で、具体的な項目名や表示内容を具体的に書くのが望ましい。よくある駄目な例が、「正しく処理されること」「問題がないこと」といったあいまいな表現。人によって解釈が異なってしまう可能性がある。


### ～感想～
実装を担当した人がそのままテストケースを記載する場合、既に機能や動作に対する主観が入ってしまい、記載内容が曖昧になったり、観点が漏れていたりすることがよくある。それを防ぐために、テストケース作成前に事前に作成方針についてチームで合意し、記載レベルのあったテストケースを作成していくことが重要だと感じた。「正しく処理されること」「問題がないこと」などといった表現は今でも使ってしまうことがあり反省。
