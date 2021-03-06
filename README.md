# teamlab_task(ToDoリスト)
__Overview__  
  このプログラムはweb上で動作する非常に扱いやすいUIデザインのToDoリストのプログラムである。  
  特徴として  
  ・UIKIT3を使った現代的なモダンなUIデザイン  
  ・画面遷移の少ない非常にスマートフォンのアプリケーションのような操作  
  ・直感的な操作をしやすいボタン  
  が挙げられる。

## Description
  UIデザインにこだわり、視覚的に操作しやすいデザインを設計。  
  ToDoに重要度の項目をつけることによって、重要度別にToDoの色が変化し、素早く重要なToDoを見分けられる。  
  検索にはキーワード検索のほか、重要度別、チェック済み、未チェック別に分類でき、調べやすい。  
  ToDoリスト、ToDoは一意なキーで管理されているため、同じ名前のデータを作成可能。
  
## Demo
__デモページ__  
https://todo-a383d.firebaseapp.com/todo_list.html  
動作確認済(２０１８年７月２０日現在の最新バージョンのもの)  
safari  
clrome  
firefox  
  
  
## Requirement
 全体の設計、構成は、Firebaseの機能を主に活用し、HostingでWebサイトをデプロイ、Realtime Databaseでデータを管理をしており、    
 入力、出力処理、データの受け渡しの処理は、htmlに埋め込んだJavaScriptで処理をしている。  
 UIはUIkit3を使用してデザイン。   
 
・このプログラムはfirebaseのhostingで一部パラメータを管理しているため、
  hosting上での動作が必須。  
  https://firebase.google.com/products/hosting/

・UIデザインにUIkit3を使用（但し、レポジトリにコンパイルされたuikit3が入っている(2018年7月19日現在のバージョン)）  
  https://getuikit.com
 
・データベースのエクスポートデータはリポジトリにあるtodo-a383d-export.jsonに記載



   仕様言語  
   ・HTML  
   ・JavaScript  
   
   フレームワーク  
   ・UIkit3  
   
   ライブラリ  
   ・Flatpickr
   
   データベース    
   ・Firebase RealtimeDatabase(NoSQL)
   
   Hosting  
   ・Firebase Hosting
  
  
## Usage
__・ToDoリストの作成__    

#### 画面の左上に新規ToDoリストをクリック。  

![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.56.24.png)

#### 作成するToDoリストのタイトルを入力（３０文字以内、英字は大文字のみ）して追加をクリック。

![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.56.56.png)

#### ToDoリストが作成され、追加される。

![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.06.png)


__・ToDoリストへ移動__ 
#### 移動したいToDoリストのタイトルの文字をクリック。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.18.png)
#### ToDoリストへ移動。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.58.00.png)

__・ToDoリストの削除__  
#### 削除したいToDoリストの行の×ボタンをクリック。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.18.png)
#### 確認画面が出るので、削除する場合は削除をクリック。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.36.png)
#### ToDoリストが削除され、削除通知が出る。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.42.png)

__・新規ToDoを作成__  
#### 左上にある新規TODOをクリックする。 
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.18.png)
#### タイトルを入力（３０文字以内、英字は大文字のみ）し、オプションとして重要度、期限を指定できる。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.58.28.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.58.37.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.58.47.png)
#### 重要度を指定すると
#### 高の場合、文字が赤に、
#### 中の場合、文字が黄色に、
#### 低の場合、文字が青に、
#### 変化する。
#### 期限を指定すると、期限の欄に指定した期限が表示される。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.59.51.png)

__・ToDoを完了させる__  
#### 完了したToDoの行の一番左側のチェックボックスをクリックする。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.32.42.png)
#### チェックが付き、完了する。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.04.15.png)

__・ToDoを削除__  
#### 削除したいToDoの行の×ボタンをクリック。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.32.42.png)
#### ToDoが削除され、削除通知が出る。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.33.19.png)

__・検索__  
#### 左上の検索をクリックし、検索したいタイトルを入力し、検索をクリック。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.29.png)
#### 検索結果が表示される。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.35.png)
#### 上の高、中、低をクリックするそれぞれの重要度に指定してあるToDoが検索される。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.41.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.47.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.53.png)
#### 下記のようなチェックされているものとされていないものを分類したい場合、上のチェック済み、未チェックをクリックすると分類される。
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.01.10.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.01.17.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.01.24.png)



  
  
## Install
・Firebaseでプロジェクトを立ち上げる。
  プロジェクト名を入力、地域、各種チェック欄に同意してチェックし、プロジェクトを作成する。
・Firebaseのhostingを作成する。   
  __1.コマンドラインを開き、npmでFirebase CLIをインストールする。__    
  `npm install -g firebase-tools`  
  
 __ 2.Firebaseにログインする。__ 　　
   `firebase  login`  
   
 __ 3.インストールが完了したら、アプリを初期化する。__   
  `firebase init`  
  
  DatabaseとHostingにチェックをつけ、Enterを押す。
  
    ? Which Firebase CLI features do you want to setup for this folder? Press Space 
      to select features, then Enter to confirm your choices. 
      ◉ Database: Deploy Firebase Realtime Database Rules
      ◯ Firestore: Deploy rules and create indexes for Firestore
      ◯ Functions: Configure and deploy Cloud Functions
     ❯◉ Hosting: Configure and deploy Firebase Hosting sites
      ◯ Storage: Deploy Cloud Storage security rules

  作成したプロジェクトを選択する。

    ? Select a default Firebase project for this directory: 
      [don't setup a default project] 
    ❯ 作成したプロジェクト (プロジェクトID) 
      [create a new project] 
  
  データベースのルールを記述するjsonファイルを作成するのでそのままEnterを押す。
  
    ? What file should be used for Database Rules? (database.rules.json) 
 
  publicディレクトリを作成するのでそのままEnterを押す。
 
    ? What do you want to use as your public directory? (public) 
 
 シングルページでは無いのでNを入力してEnterを押す。
 
    ? Configure as a single-page app (rewrite all urls to /index.html)? (y/N) N  
  
  __4.アプリを初期化したら、ディレクトリのルート(デフォルトはpublic)にtodo.html,todo_list.htmlとcss,jsディレクトリを追加します。__    
    
    
  __5. todo.htmlとtodo_list.htmlのファイルのソースコードの一部を変更します。(自分のFirebaseのプロジェクトIDをURLに書き込む)__   
  
  todo.html  
    
    <a class="uk-navbar-item uk-logo uk-active" href="https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo_list.html">ToDoリスト</a> 
    
    <a class="uk-button" href="https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo_list.html" onclick="javascript:window.history.back(-1);return false;">リストに戻る</a>
    
    
  todo_list.html  
  
    <a class="uk-navbar-item uk-logo uk-active" href="https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo_list.html">ToDoリスト</a>  
    
    window.location.href = 'https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo.html';  
  
  
  __6.Databaseのルールを変更.__  
  自由に書き換えられるようにdatabase.rules.jsonのコードを以下のように書き換える。
  
    {
      "rules": {
        ".read": "auth != true",
        ".write": "auth != true"
      }
    }
  
  __7.webサイトをデプロイする.__  
  `firebase deploy`  
 

## Licence
This project is licensed under the terms of the MIT license.


