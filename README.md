## URL  
 - Uniform Resource Locator　の略  
 - ネットワーク上の「情報の住所」
### クエリ文字列　　
 - URIの構文の一つ、クエストストリングとも呼ばれる
 - クライアントがサーバーに送信するデータを、送信先を指定するURLの末尾に特定の形式で表記したもの
### パスパラメーター(パス変数)  
 - 特定の情報を表示するために活用される
 - 一意なリソースを指定し、省略はできない  
  
**クエリ文字との違い**   
- URIでドメインの後、「?」の前に来るものがパスパラメータ、後に来るのがクエリ文字列


## HTTPメソッド
  - クライアントが行いたい処理をサーバに伝える為のもの  
 
    
    >` GET `    サーバーへ指定したリソースの送信を要求  
    >` POST `   クライアントからデータを送信するためのもの  
    >` PUT `    リソースの内容の更新とリソースの作成  
    >` PATCH `  リソースへの部分的な変更  
    >` DELETE ` 指定したリソースを削除  


## HTTPステータスコード
  - 一番上のレスポンス行で表示される3桁の番号のこと
 
 | 番号 | 内容 |
 ----|----
 | 200-OK | リクエストが成功した |
 | 201-Created |リクエストの成功とリソースの作成の完了  |
 | 400-BadRequest | クライアント側にエラーがあるためリクエストを処理しない |
 | 404-NotFound | リクエストされたリソースを見つけることができない |
 | 500-InternalServerError | サーバーでリクエストの実行を妨げるエラーが起きた |

#### リクエストヘッダー
 - リクエストに関する追加情報やクライアント自身の情報を付与するためのヘッダー
#### リクエストボディ
 - 必要に応じて補足情報が書かれる
#### レスポンスヘッダー
 - レスポンスについての追加情報を含むヘッダー
#### レスポンスボディ
 - クライアントに送るデータ
### JSONとは
 - JavaScriptObjectNOtation の略
 - 異なるプログラミング言語間でデータをやり取りするための共通のデータ記述形式
 - JavaScript上で値を取り扱うためのフォーマットだったが、バックエンドと通信する際のフォーマットとして利用されるようになった  
  
  
[参照1](https://e-words.jp/w/HTTP.html)  
[参照2](https://developer.mozilla.org/ja/docs/Web)
  
# 映画情報  
```json
````
[  
 &emsp; {  
   &emsp; "title":"グレイテスト・ショーマン",  
   &emsp; "director":"マイケル・グレイシー",  
   &emsp; "published_year":"2017"  
 &emsp; },  
 &emsp; {  
   &emsp; "title":"エスター",  
   &emsp; "director":"ジャウム・コレット＝セラ",  
   &emsp; "published_year":"2009"  
  &emsp; },  
  &emsp; {  
   &emsp; "title":"告白",  
   &emsp; "director":"中島哲也",  
   &emsp; "published_year":"2010"  
  &emsp; }  
]
````
