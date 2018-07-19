# teamlab_task(ToDoリスト)
Overview  
  このプログラムはweb上で動作する非常に扱いやすいUIデザインのToDoリストのプログラムである.  
  特徴として  
  ・UIKIT3を使った現代的なモダンなUIデザイン  
  ・画面遷移の少ない非常にスマートフォンのアプリケーションのような操作  
  ・直感的な操作をしやすいボタン  
  が挙げられる。

## Description


## Demo
デモページ  
https://todo-a383d.firebaseapp.com/todo_list.html


## Requirement
・このプログラムはfirebaseのhostingで一部パラメータを管理しているため、
  hosting上での動作が必須。  
  https://firebase.google.com/products/hosting/

・UIデザインにUIkit3を使用（但し、レポジトリにコンパイルされたuikit3が入っている(2018年7月19日現在のバージョン)）  
  https://getuikit.com


## Usage

## Install
・Firebaseのhostingを作成する。   
  1.コマンドラインを開き、npmでFirebase CLIをインストールする。    
  `npm install -g firebase-tools`
  
  2.Firebaseにログインする。　　
   `firebase  login`
   
  3.インストールが完了したら、アプリを初期化します。  
  `firebase init`
  ホスティングを
  ? Which Firebase CLI features do you want to setup for this folder? Press Space 
to select features, then Enter to confirm your choices. 
◉ Database: Deploy Firebase Realtime Database Rules
 ◯ Firestore: Deploy rules and create indexes for Firestore
 ◯ Functions: Configure and deploy Cloud Functions
❯◉ Hosting: Configure and deploy Firebase Hosting sites
 ◯ Storage: Deploy Cloud Storage security rules
 
? Select a default Firebase project for this directory: 
  [don't setup a default project] 
❯ todo (todo-a383d) 
  [create a new project] 
  
 ? What file should be used for Database Rules? (database.rules.json) 
 
 ? What do you want to use as your public directory? (public) 
 
? Configure as a single-page app (rewrite all urls to /index.html)? (y/N) N


 
  
  4.アプリを初期化したら、ディレクトリのルート(デフォルトはpublic)にtodo.html,todo_list.htmlを追加します。  
  
  5. todo.htmlとtodo_list.htmlのファイルのソースコードの一部を変更します。(自分のFirebaseのプロジェクトIDをURLに書き込む)  
  
  todo.html
    
    <a class="uk-navbar-item uk-logo uk-active" href="https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo_list.html">ToDoリスト</a> 
    
    <a class="uk-button" href="https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo_list.html" onclick="javascript:window.history.back(-1);return false;">リストに戻る</a>
    
    
  todo_list.html
  
    <a class="uk-navbar-item uk-logo uk-active" href="https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo_list.html">ToDoリスト</a>  
    
    window.location.href = 'https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo.html';
  
  
  6.webサイトをデプロイする.
  `firebase deploy`
 
　

## Contribution

## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)

## Author

[tcnksm](https://github.com/tcnksm)
