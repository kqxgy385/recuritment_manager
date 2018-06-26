# recuritment_manager

採用の選考者を管理することを目的とした作りかけのツールです。 <br>
会社で使ってもらいたいと思って作り始めましたが、色々あって頓挫しました。 <br>
自分用に拡張していこうと思います。<br>
最も苦労したのはDjangoはSQLiteが標準搭載になっているが自分はMySQLで書きたかったのでドライバを入れ直したら、herokuのDBはデフォルトではPostgreなので、MySQLを使おうとすると設定を変更する必要があり、インフラ側の設定変更が全く分からず時間もなかったので渋々Posgre対応にしたことです。

以下でログインできます。<br>
ID: u13641 <br>
Pass: dreU1tZJ

https://test-app-20180622005216.herokuapp.com/accounts/login/

## 主な画面
### 採用候補者一覧
 -各カラムソートができます<br>
 -IDをクリックすると更新に遷移します。<br>
 -「アーカイブに移動する」でアーカイブに遷移します。

### 採用候補者更新
 -一覧から遷移します<br>
 -選考者情報を更新できます<br>
 -連絡先は@以降を入力しないとバリデーションエラーになります

### 採用候補者追加
 -新規選考者を追加できます
 
### 面接日程追加
 -候補者の日程を更新できます<br>
 -候補者名で選択できます

### 過去選考者一覧
 -一覧から遷移できます<br>
 -「一覧に戻す」でアーカイブから消すことができます

## できないこと
 -ログイン情報ごとにアカウントを分ける<br>
 -アカウントごとに権限をつける<br>
 -過去の面接情報が履歴表示される<br>
 -チャット<br>
 etc...
 
 ## 使っている技術
Python 3.6.3<br>
Django 2.0.6<br>
heroku<br>
PostgreSQL
