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


