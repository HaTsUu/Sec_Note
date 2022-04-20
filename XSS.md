## XSSの詳細な情報

・[XSS MIND MAP @Jackmasa](https://raw.githubusercontent.com/cyberspacekittens/XSS/master/XSS2.png)<br>
・[HTML Security CheatSheet](https://html5sec.org/)


## [Polyglot](https://github.com/0xsobky/HackVault/wiki/Unleashing-an-Ultimate-XSS-Polyglot)
様々な種類のペイロードと難読化手法を1つの攻撃として組み合わせる

## [BeEf(Browser Explotation Framework)](http://beefproject.com/)
XSSをさらに強力にするツール。<br>
標的のブラウザにJavaScriptペイロードを注入し、ユーザーのシステムを感染させる。<br>
キャンペーン、ユーザーの追跡、認証情報のキャプチャ、クリックジャッキング、タブナッピングによる攻撃を実行できる。
 
## ブラインドXSS
ブラインドは忍耐を要する攻撃。<br>
蓄積型XSSのペイロードが攻撃者やユーザーからはみえず、システム管理者やバックエンドオペレータにだけ見える攻撃。<br>
ブラインドXSSの検証には[XSSHunter](http://xsshunter.com)を使うことができる。

## DOM(Document Object Model)ベースのXSS
DOMベースのXSSが可能になるのは、アプリケーションがDOMを通じて動的にHTMLを組み立てている箇所で、悪意を持つスクリプトを注入できる場所。<br>
XSSが何度でも通じる大きな理由の一つは、タグや特定の文字の単なるフィルタリングではないから。<br>
ペイロードが特定の言語やフレームワークを対象としたものである場合、XSSに対する防衛は困難を極める。<br>
脆弱性に関しては、言語ごとに奇異な点がある。<br>
フィルタをかわしてJavaScriptを挿入するには[JsFuck](http://www.jsfuck.com/)などをを使って難解な表記を利用する(Node.js,pugのみ？)

## XSSからシェルを取得
CMS(Content Management System)などでユーザーからシステム管理者に昇格するスタイルのXSS。<br>
ウォークスルーサンプルコード[Hans-Michael VarBaekのGITリポジトリ](https://github.com/VarBaek/xsser)。
このリポジトリはXSS to RCE攻撃を再現するためのサンプルや動画を提供してくれている。<br>
