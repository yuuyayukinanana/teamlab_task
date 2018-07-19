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
・Firebaseのhostingを作成する 
  1.コマンドラインを開き、npmでFirebase CLIをインストールします。  
  `npm install -g firebase-tools`
  
  2.インストールが完了したら、アプリを初期化します。  
  `firebase init`
  
  3.アプリを初期化したら、ディレクトリのルート(デフォルトはpublic)にtodo.html,todo_list.htmlを追加します。  
  
  4. todo.htmlとtodo_list.htmlのファイルのソースコードの一部を変更します。  
    todo.html
    <a class="uk-navbar-item uk-logo uk-active" href="https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo_list.html">ToDoリスト</a>
    window.location.href = 'https://自分のFirebaseのプロジェクトID.firebaseapp.com/todo.html';
    
    <a class="uk-navbar-item uk-logo uk-active" href="https://todo-a383d.firebaseapp.com/todo_list.html">ToDoリスト</a>
    <a class="uk-button" href="https://todo-a383d.firebaseapp.com/todo_list.html" onclick="javascript:window.history.back(-1);return false;">リストに戻る</a>
    todo_list.html
  
  
  3.`firebase deploy`
 
　

## Contribution

## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)

## Author

[tcnksm](https://github.com/tcnksm)
