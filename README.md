## Twitter的なアプリケーション

### システム要件
* VirtualBox(Vagrant)
  * Linux
    * MySQL
    * Passenger(ここにApacheも含める)
* Ruby
* Sinatora

#### システム要件について
* ansibleは余力があれば
* 完成まで行かなくていいが、どのように実施するかを考慮しておくもの
  * レプリケーション
  * DBのスケールアウト
  * APサーバが増えること


### アプリケーション要件
* ログインできる
* セッションを保持できる
* つぶやける
* タイムラインが見れる
* 他のユーザーをフォロー／リムーブできる

#### アプリケーションについて
* 最低限、最小限のアプリケーション構成
* デザインもなし
* ツイート、更新など全て静的に行う
