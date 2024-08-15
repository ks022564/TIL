# java Tips

## 2024-08-12
### Javaを導入
### ソースコードの基本ルール
  - Javaのソースコードを書く際には、読みやすさ、保守性、効率性を考慮する。
    - インデントとスペース
インデントにはスペースまたはタブを使用: インデントにはスペース（通常は4スペース）かタブを使用します。プロジェクトで統一したスタイルを使用することが重要。

    - ブロックの開始と終了: ブロックの開始（{）はブロックを開始する行の終わりに書き、終了（}）はブロックの最後に書く。
- コメント
  -  コードの意図や動作を説明するためにコメントを適切に使用する。ただし、過剰なコメントは避け、読みやすいコードを書くことを心がける。

     1. シングルラインコメント: // を使って一行コメントを書く
     2. マルチラインコメント: /* */ を使って複数行のコメントを書く

## 2024-08-14
### JAVA 変数
- データ型。データ型とは、変数に格納するデータの種類のことです。
Rubyカリキュラムですでに学習したように、「数値としての1」と「文字としての1」はプログラムの上では異なるものとして扱われます。
データ型は、このような「数値」や「文字」といった種類をより細かく定めたもので、Javaの基本データ型には8つの種類があります。
  1. boolean 1bit	true あるいは false
  2. char	16bit	文字
  3. byte	8bit	整数（扱える範囲は -128～127）
  4. short	16bit	整数（扱える範囲は-32,768～32,767）
  5. int	32bit	整数（扱える範囲は-2,147,483,648～2,147,483,647）
  6. long	64bit	整数（扱える範囲は-9223372036854775808～9223372036854775807）
  7. float	32bit	小数（精度低）
  8. double	64bit	小数（精度高）
  -  よく使用するのは5と6

- 静的型付け言語　動的型付け言語
  - 静的型付け言語。 動的型付け言語は、プログラムの実行時に変数のデータ型を決定する方式で、Rubyはこちらに含まれます。
  -  動的型付け言語。静的型付け言語は、動的型付け言語とは異なり、変数のデータ型を最初に決定したら変更できない仕組みです。Javaはこちらに含まれます。

### 演算子
- Rubyと同じ

### 配列とリスト
#### 配列
- Rubyと同様にJavaにも配列がありますが、Rubyの配列とは性質が異なります。
Javaの配列は、格納する要素の数を最初に決める必要があり、かつ後で要素数を変更することができません。
- 配列の使い方
  1. 配列の宣言を行う  
  2. 配列の要素を作成し、配列に代入する  
  3. 配列の要素に値を代入する  

#### リスト
- リストは、Rubyの配列と似たデータ管理の仕組みです。
以下の特徴があります。
要素を順序づけて管理する
要素を事後的に追加したり削除できる
また、Javaのリストには、以下の2種類があります。
ArrayList
LinkedList

 1. ライブラリをインポートする  
 2. ArrayListの宣言を行う
 3. ArrayListに値を代入する
 4. ArrayListから要素を取り出す

### 条件分岐
- Rubyと同じ

### 繰り返し処理
- 拡張for文
  - for ( 要素を格納する変数宣言  :  配列あるいArrayListの変数名) {
  取り出した要素を使用して行う処理}
  1. 配列、あるいはArrayListから要素を1つ取り出す
  2. 取り出した要素を変数に代入する
  3. {}内の処理を行う
  4. 配列、あるいはArrayListの要素数分だけ処理を繰り返す

### メソッド
#### メインメソッド
- mainメソッドには以下の２つのルールがあります。
① ファイルを実行するとmainメソッドが実行される
② mainメソッドの引数などは、必ず決められた通りに記述する必要がある

#### 一般的なメソッド
- メソッドを定義するための構文は以下のようになっています。
  - アクセス修飾子 static修飾子 返り値のデータ型　メソッド名() {
  // 行いたい処理
}