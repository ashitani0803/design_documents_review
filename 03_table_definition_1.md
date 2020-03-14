# テーブル定義書1
## 全体
- テーブルの命名規則に従っていない。
- idがない。

## Admin
- PKがない。
- カラム名の前にadminがついてる。

## Users
- カラム名の前にuserがついてる。
- 住所に関するカラムが2つある。
- member_statusがstring型になっている。
- 郵便番号と電話番号がinteger型になっている。

## Products
- アーティストID、レーベルID、ジャンルIDにFKの設定がない。
- 在庫数カラムがある。
- ディスクIDを持っている。
- カラムの前にcdがついてる。

## Discs
- 外部キーはproducts_idになっている。
- track_numではディスクをディスクを特定できない。

## Songs 
- PKがない。
- 曲名カラムかintegerになっている。

## Labels
- PKがない。
- products_idがある。

## Artists
- PKがない。
- products_idがある。

## Genre
- Pkがない。
- products_idがある。
- ジャンル名カラムがinteger型になっている。
- テーブル名が単数系になっている。

## CartItem
- PKがない。
- 外部キーがproducts_idになっている。
- buy numはスペースが入っていて、カラムとして使用できない。
- テーブル名が単数系になっている。
- 小計金額カラムがある。

## Buy
- テーブル名が単数系になっている。
- 購入詳細IDを持っている。
- 支払い方法のカラムがstring型になっている。
- stockカラムが支払い合計になっている。
- 購入日カラムがある。
- 配送先住所と宛名のカラムがない。

## BuyDetails
- buy numはスペースが入っていて、カラムとして使用できない。
