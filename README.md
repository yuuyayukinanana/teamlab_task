# teamlab_task(ToDoリスト)
__Overview__  
  このプログラムはweb上で動作する非常に扱いやすいUIデザインのToDoリストのプログラムである。  
  特徴として  
  ・UIKIT3を使った現代的なモダンなUIデザイン  
  ・画面遷移の少ない非常にスマートフォンのアプリケーションのような操作  
  ・直感的な操作をしやすいボタン  
  が挙げられる。

## Description
  
  
## Demo
__デモページ__  
https://todo-a383d.firebaseapp.com/todo_list.html
  
  
## Requirement
・このプログラムはfirebaseのhostingで一部パラメータを管理しているため、
  hosting上での動作が必須。  
  https://firebase.google.com/products/hosting/

・UIデザインにUIkit3を使用（但し、レポジトリにコンパイルされたuikit3が入っている(2018年7月19日現在のバージョン)）  
  https://getuikit.com
  
  
## Usage
__・ToDoリストの作成__    

#### 画面の左上に「新規ToDoリスト」をクリック。  

![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.56.24.png)

#### 作成するToDoリストのタイトルを入力（３０文字以内）して追加を押す。

![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.56.56.png)

#### ToDoリストが作成され、追加される。

![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.06.png)


__・ToDoリストへ移動__  
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.18.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.58.00.png)

__・ToDoリストの削除__  
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.18.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.36.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.42.png)

__・新規ToDoを作成__  
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.57.18.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.58.28.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.58.37.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.58.47.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%201.59.51.png)

__・ToDoを完了させる__  
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.32.42.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.04.15.png)

__・ToDoを削除__  
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.32.42.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.33.19.png)

__・検索__  
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.29.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.35.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.41.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.47.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.00.53.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.01.10.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.01.17.png)
![Alt text](https://github.com/yuuyayukinanana/teamlab_task/blob/master/images/スクリーンショット%202018-07-20%202.01.24.png)



  
  
## Install
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
  
  __4.アプリを初期化したら、ディレクトリのルート(デフォルトはpublic)にtodo.html,todo_list.htmlを追加します。__    
    
    
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


