# projectの環境設定

## Ruby環境の構築
```
$sudo apt-get install git build-essential libssl-dev
$git clone https://github.com/sstephenson/rbenv.git ~/.rbenv
$git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
$vim ~/.bashrc
```

`最下行に下記を追記`
```
$export PATH="$HOME/.rbenv/bin:$PATH"
$eval "$(rbenv init -)"

$source ~/.bashrc
$rbenv install 2.4.2
$rbenv global 2.4.2
$gem install bundler
```

## jekyllのインストール
```
$sudo apt-get update
$sudo apt-get install ruby ruby-dev make gcc
$sudo gem install jekyll bundler
$jekyll new my-awesome-site //jekyll でサイトの自動作成
$jekyll serve //ローカルサーバーで動かしてみる
```
## githubのアカウントの作り方
Start building を選択する.
Sign up with GitHub を選択.
Create an accountを選択.
User name, Email address, Passwordを入力する.
プランを選択.
確認メールが来るので、Verify email address を選択.
Welcome to GitHub!

## githubでチームのプロジェクトを共有する
自分のID(ユーザーID)を作成者に伝えて招待される（招待メール届く）
```
$git clone -----(作成者のページ「ダウンロードまたはクローン」から)
```
## gitの環境構築
https://qiita.com/varmil/items/9b0aeafa85975474e9b6
または「git status 100回」で検索
https://github.com/git/git/tree/master/contrib/completion
を参考にします
```
$git clone https://github.com/git/git.git
$cp git/contrib/completion/git-completion.bash ./       //gitコマンド補完スクリプト
$mv git-completion.bash .git-completion.bash        //ファイルを隠しファイルに変更
$chmod a+x ~/.git-completion.bash       //権限付与
 
$cp git/contrib/completion/git-prompt.sh ./
$mv git-prompt.sh .git-prompt.sh 
$chmod a+x ~/.git-prompt.sh
$source .bashrc
```
