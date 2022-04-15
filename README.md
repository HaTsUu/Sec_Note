# セキュリティノート
最近いろいろなツールや単語がでてきて忘れちゃうことがあるので
自分用に作りました。

## サブドメイン列挙
|  名前  |  説明  |
|  ----  |  ----  |
|  Knock  |Knockはワードリストに精度が左右される  |
|  DiscoverScript  |要調べ  |
|  Sublist3r  |検索エンジンを使用してサブドメインを列挙する。検索クエリを使用するため、ブラックリストに載ってしまう場合あり  |
|  SubBrute  |高い匿名性と高速スキャンを実現した。標的のネームサーバーにトラフィックを直接送信しない。<br>DNSレコードを列挙するDNSスパイダー機能も実行する（massDNSを使えば高い性能になる)  |

## GIT 情報収集
|  名前  |  説明  |
|  ----  |  ----  |
|  TruffleHog  |Gitのコミットりれきとブランチでエントロピーの高い文字列をスキャンして出力する。  |
|  Git-All-Secrets  |大きな組織を調べるときに使う。セットアップが少しめんどくさい。TruffleHogとrepo-supervisorを使ってスキャンを行う。  |

## クラウド
|  名前  |  説明  |
|  ----  | ----  |
|  slurp  | バケットの列挙。キーワードまたはリストを受け取り複数の組み合わせを行い、パケットの検出を試みる。  |
|  BucketFinder  |パケットの特定と内容をすべてダウンロードして解析できるようにする。  |

## AWSアクセスキーIDの取得
  AWSアカウントを作成→ログイン→アカウント名をクリック→[セキュリティ認証情報]→
  [アクセスキー(アクセスキーIDとシークレットアクセスキー)]をクリックする

## S3を調べてバケットの内容をダウンロードするツール
・awscli

## AWSのパーミッションが正しく設定されているか確認するツール
・s3api

## 脆弱なサブドメインをチェックする
・Tko-subs(https://github.com/anshumanbh/tko-subs)

## ドメイン奪取
・HostileSubBruteforcer(https://github.com/nahamsec/HostileSubBruteforcer)<br>
・AutoSubTakeover(https://github.com/JordyZomer/autoSubTakeover)

## AWS脆弱性にもっと知りたい場合
・http://flaws.cloud/

## メアド攻撃？※要チェック
・SimplyEmail

## OSINT(Open source Intelligence?)リンク集
・https://github.com/IVMachiavelli/OSINT_Team_Links

## OSINT Framework
・http://osintframework.com/

## OWASP Tsting Guide
・https://www.owasp.org/index.php/OWASP_Testing_Guide_v4_Table_of_Contents
・https://www.owasp.org/images/1/19/OTGv4.pdf

## ツール等の一覧
脆弱性診断等に使うツールや拡張機能。
まとめてあったほうが便利なので別でまとめています。
|  名前  |  説明  |
|  ----  |  ----  |
|  [Wappalyzer](https://www.wappalyzer.com/) |表示中のWebページで利用されているソフトウェアやサービス、フレームワークなどを一覧表示する。<br>拡張機能などで使用可能。  |
|  [BuiltWith](https://builtwith.com/)   |閲覧中のWebページに利用されている技術を調査できる拡張機能。 |
|  [Retire.js] (https://retirejs.github.io/retire.js/) |Webアプリケーションに脆弱なJavaScriptライブラリを使用しているかを確認する。  |
|  [BurpSuite](https://portswigger.net/burp)  |ローカルプロキシツール。キャプチャをしたり、リクエストの値を変えたりと便利ツール。コミュニティ版とプロ版がある。  |
|  [OWASP Zap](https://www.zaproxy.org/)  |オープンソースのWebアプリケーションセキュリティスキャナーBurpSuiteと同様便利ツール※要調べ  |
|  DirBuster  |Webアプリケーションのファイルやフォルダーを発見するためのツール。Webブルートフォースツール。  |
|  [FeroxBuster](https://github.com/epi052/feroxbuster)  |Webブルートフォースツール。DirBusterと似たようなツール。DirBusterなどが使えないときに使う。  |
|  [GoBuster](https://github.com/0J/gobuster)  |軽量で高速なWebブルートフォースツール。サブドメイン等も列挙ができる。GUI版もある。  |


 

## 攻撃の手口
|  名前  |  説明  |
|  ----  |  ----  |
|  スピアフィッシング  |成功率の高い攻撃の一種。特定の人を狙ってメールなどで攻撃をする。<br>ソーシャルエンジニアリングなどで人物の情報を収集することを中心としている。  |
|  XSS(クロスサイトスクリプティング) [詳細](/XSS.md)  |Webアプリケーションの脆弱性もしくはそれを利用した攻撃。<br>攻撃者がそこに悪質なサイトへ誘導するスクリプトを仕掛けることで、サイトに訪れるユーザーの個人情報などを詐取する。ブラウザによって動作が大きく異なる場合がある。<br>XSS作成参考:(https://github.com/foospidy/payloads/tree/master/other/xss)<br>(https://www.owasp.org/index.php/XSS_Filter_Evasion_Cheat_Sheet)  |
|  キーロガー  |キーボードから入力した文字情報などを記録するソフトウェアだが、悪用して個人情報などを盗むことも可能。  |


## セキュリティ単語集etc...

|  名前  |  説明  |
|  ----  |  ----  |
| OWASP  |Webアプリケーションセキュリティの分野で自由に利用できる記事、方法論、ドキュメント、ツール、およびテクノロジを作成するオンラインコミュニティ。<br>https://owasp.org/www-chapter-japan/  |
|  スナップショット  |スナップショットとは、NAS上のファイルやフォルダの状態を定期的に記録・保存しておく技術。参考:(https://note.com/qnap/n/n2b9f5ff6bc11)  |




