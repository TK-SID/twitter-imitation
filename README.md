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

## Vagrant環境構築
Vagrant環境構築手順
* VirtualBox入れる
* Vagrant入れる
* CentOS6.5のBoxを入れる
  * `$ vagrant box add centOS6.5 https://github.com/2creatives/vagrant-centos/releases/download/v6.5.3/centos65-x86_64-20140116.box`
* Vagrant初期化
  * `$ mkdir twitter-imitation`
  * `$ cd twitter-imitation`
  * `$ vagrant init centOS6.5`
* SSHでログイン
  * `vagrant ssh`
