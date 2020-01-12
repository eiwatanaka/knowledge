## 1. はじめに
ここ2年程、C#を使ったプロジェクトに携わっています。
LINQがこれまた便利なもので、コードがシンプルになるためガシガシ使っているのですが、
備忘録のためよく使うLINQをまとめておきたいかと思います。

**※以下のサイトでC#のビルド・実行が簡単に行えます。ちょっとしたお勉強のときにとても便利！**
https://dotnetfiddle.net/


## 2. LINQとは
Language Integrated Queryの略です。
SQLのクエリのような表記を使うことで、データに対する検索や操作を簡単に直感的に行うことができます。
SQLとは違う！！と怒る方もいるようですが、私は気にしません。
DQとFFの違いと思ってください。(←大嘘)


## 3. よく使ってきたLINQ

### 3-1. Where
指定した条件に一致する要素のみを抽出します。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.Where(v => v % 2 == 0); // 結果：2, 4
```

### 3-2. Any
要素が含まれているかを調べます。条件を指定することもできます。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.Any(); // 結果：true
values.Any(v => v == 3); // 結果：true
values.Any(v => v == 7); // 結果：false 
```

### 3-3. Contains
指定した要素が含まれているかを調べます。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.Contains(3); // 結果：true
values.Contains(7); // 結果：false 
```

### 3-4. First
先頭要素を取得します。条件を指定することもできます。
値が取得できない場合はエラーとなります。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.First(); // 結果：1
values.First(v => v % 2 == 0); // 結果：2 
values.First(v => v % 2 == 9); // 結果：エラー  
```

### 3-5. FirstOrDefault
先頭要素を取得します。条件を指定することもできます。
値が取得できない場合は型の初期値が返ります。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.FirstOrDefault(); // 結果：1
values.FirstOrDefault(v => v % 2 == 0); // 結果：2 
values.FirstOrDefault(v => v % 2 == 9); // 結果：0  
```

### 3-6. Last
末端要素を取得します。条件を指定することもできます。
値が取得できない場合はエラーとなります。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.Last(); // 結果：5
values.Last(v => v % 2 == 0); // 結果：4
values.Last(v => v % 2 == 9); // 結果：エラー  
```

### 3-7. LastOrDefault
末端要素を取得します。条件を指定することもできます。
値が取得できない場合は型の初期値が返ります。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.LastOrDefault(); // 結果：5
values.LastOrDefault(v => v % 2 == 0); // 結果：4 
values.LastOrDefault(v => v % 2 == 9); // 結果：0  
```

### 3-8. Max
最大要素を取得します。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.Max(); // 結果：5
```

### 3-9. Min
最小要素を取得します。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.Min(); // 結果：1
```

### 3-10. ElementAt
指定したインデックス位置にある要素を取得します。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.ElementAt(2); // 結果：3
```

### 3-11. Distinct
重複する要素を除外します。

```C#
var values = new[] { 1, 2, 3, 1, 4, 3, 5 };
values.Distinct(); // 結果：1, 2, 3, 4, 5
```

### 3-12. Select
変換関数を適用した結果を取得します。

```C#
var values = new[] { 1, 2, 3, 4, 5 };
values.Select(v => v * v); // 結果：1, 4, 9, 16, 25
```

## 4. おわりに
LINQを使ってシンプルなコードを書いていきましょう！
他にもありましたら随時更新させて頂きます。
