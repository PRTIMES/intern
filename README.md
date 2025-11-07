# PR TIMES 学生インターン課題

「[ISUCON](https://isucon.net)」は、LINE株式会社の商標または登録商標です。

[PR TIMESで実力を上げたい学生インターンを募集します | PR TIMES 開発者ブログ](https://developers.prtimes.jp/2021/08/25/prtimes-intern-202108/)

## 課題

* [catatsuy/private-isu](https://github.com/catatsuy/private-isu) を動かしてください
  * 言語は複数の言語が用意されており、デフォルトはRubyです
    * PR TIMES社内ではPHPが利用されているため、**必ずPHPを利用**してください
    * PHPは追加の手順が必要なのでREADMEをよく読んでください
  * AWSアカウントがあればAMIで起動するのが一番簡単ですが、クレジットカードと利用料が必要です
  * 手元で動かす方法や[Docker Compose](https://www.docker.com/)・[Vagrant](https://www.vagrantup.com/)を使う方法もあります
    * 仮想マシンが起動できない場合、BIOSの設定を確認してください
  * AWSか手元で動かすかは自由ですが、必ずどちらかの方法で動かしてください
* ブラウザからアプリケーションが表示されるか確認して下さい
  * AWSを利用する場合は80番ポートが公開されているか確認してください
  * それ以外の方法の場合、セキュリティ設定に気をつけてください
* benchmarkerを動かして正しく動いているか確認してください
  * 正しく実行ができていれば`{"pass":true,"score":1710,"success":1434,"fail":0,"messages":[]}`のようなJSONが出力されます
    * passがtrueであることと、scoreの数値を大きくすることが重要です
  * この時のbenchmarkerの出力をメモしておいてください
* 自分のGitHubアカウントを使って空のリポジトリを作ってください
  * 名前はわかりやすければ何でも構いません
* `/home/isucon/private_isu/webapp/`ディレクトリの中で`git init`して、先程作ったあなたのリポジトリにpushしてください
  * AMI・Vagrant以外の方法で起動している場合はwebappディレクトリの中で`git init`してください
  * あなたが行った変更の差分が分かるように必ず変更を行う前に`git init`をしてコミットするのを忘れないで下さい
* アプリケーションのソースコードに複数の変更を加えてscoreを上げてください
  * 変更を行ったら変更内容毎にPull Requestにしてください
  * Pull Requestは必ずmergeしてください
  * Pull Requestのdescriptionに変更を行う前のscoreと、変更した後のscoreを記載してください
  * Pull Requestのdescriptionになぜその変更を行ったのか説明を書いてください
    * 箇条書きなどで書いてください
    * 分かりやすければ形式は問いません
  * MySQLのスキーマを変更した場合は変更内容をPull Requestのdescriptionに記入してください
    * 現在のスキーマを事前にコミットしておくなど、工夫してください
    * こちらの変更も重要な変更ですが、ソースコードの変更をするPull Requestも別に用意してください
  * ミドルウェアのパラメータの変更をした場合は変更内容をPull Requestのdescriptionに記入してください
    * 現在の設定を事前にコミットしておくなど、工夫してください
    * こちらの変更も重要な変更ですが、ソースコードの変更をするPull Requestも別に用意してください
* README.mdに最終的なスコアを記述してください
  * 総括など自由に記述してください

## 注意点

* 変更内容自体よりもソースコードに対して変更が行えるか、プログラムが実行できるかを見る選考です
  * スコアが変わらなかった場合はなぜ変わらなかったのか考察してください
* ISUCONはスコアを競うものですが、今回の選考にスコアは関係ありません
  * ただし初期のスコアと最終的なスコアは必ずREADME.mdに記述しておいてください
* 変更内容はいくつ作っても大丈夫です
  * 変更内容はそれぞれPull Requestを作ってわかりやすくしてください
* 解説ブログや本を参照しても大丈夫です
  * ただし実際に適用して、スコアを計測し、変更内容を自分の言葉で説明すること

## 参考URL

［2016年開催時のブログ］

* [ISUCON6出題チームが社内ISUCONを開催！AMIも公開！！ - pixiv inside [archive]](https://devpixiv.hatenablog.com/entry/2016/05/18/115206)
* [社内ISUCONを公開したら広く使われた話 - pixiv inside [archive]](https://devpixiv.hatenablog.com/entry/2016/09/26/130112)

［2021年開催時のブログ］

* [社内ISUCON “TIMES-ISUCON” を開催しました！ | PR TIMES 開発者ブログ](https://developers.prtimes.jp/2021/06/04/times-isucon-1/)

Git/GitHubの使い方

* [サル先生のGit入門〜バージョン管理を使いこなそう〜【プロジェクト管理ツールBacklog】](https://backlog.com/ja/git-tutorial/)
