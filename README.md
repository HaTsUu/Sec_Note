# セキュリティノート
本とかの用語やツールをまとめています。
自分用ですが誰かの役に立てたら嬉しいです

## ほかの人のチートシート等
下にスクロールしてみるのめんどくさいからまとめます<br>
・https://github.com/sanposhiho/MY_CHEAT_SHEET<br>
・https://github.com/yukitsukai47/PenetrationTesting_cheatsheet<br>
・https://github.com/OWASP/www-chapter-japan/tree/master/secreq<br>
・https://kakyouim.hatenablog.com/entry/2020/04/17/182049

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
・https://www.owasp.org/index.php/OWASP_Testing_Guide_v4_Table_of_Contents<br>
・https://www.owasp.org/images/1/19/OTGv4.pdf

## ツール等の一覧
脆弱性診断等に使うツールや拡張機能。
まとめてあったほうが便利なので別でまとめています。
|  名前  |  説明  |
|  ----  |  ----  |
|  [Metasploit](https://www.metasploit.com/)  |オープンソースで、脆弱性、ペネトレーションテスト、侵入検知システム、シェルコードのアーカイブ、アンチフォレンジクスなどができる |
|  [Wappalyzer](https://www.wappalyzer.com/) |表示中のWebページで利用されているソフトウェアやサービス、フレームワークなどを一覧表示する。<br>拡張機能などで使用可能。  |
|  [BuiltWith](https://builtwith.com/)   |閲覧中のWebページに利用されている技術を調査できる拡張機能。 |
|  [Retire.js](https://retirejs.github.io/retire.js/) |Webアプリケーションに脆弱なJavaScriptライブラリを使用しているかを確認する。  |
|  [BurpSuite](https://portswigger.net/burp)  |ローカルプロキシツール。キャプチャをしたり、リクエストの値を変えたりと便利ツール。コミュニティ版とプロ版がある。  |
|  [OWASP Zap](https://www.zaproxy.org/)  |オープンソースのWebアプリケーションセキュリティスキャナーBurpSuiteと同様便利ツール※要調べ  |
|  DirBuster  |Webアプリケーションのファイルやフォルダーを発見するためのツール。Webブルートフォースツール。  |
|  [FeroxBuster](https://github.com/epi052/feroxbuster)  |Webブルートフォースツール。DirBusterと似たようなツール。DirBusterなどが使えないときに使う。  |
|  [GoBuster](https://github.com/0J/gobuster)  |軽量で高速なWebブルートフォースツール。サブドメイン等も列挙ができる。GUI版もある。  |
|  [fuff](https://github.com/ffuf/ffuf) |WEBファジングツール。Gobusterなどのブルートフォースツールと同じくくり。 早いらしい |
|  [BeEF](http://beefproject.com/)  |XSSをさらに強力にするツール。キャンペーン、ユーザーの追跡、認証情報のキャプチャなどができる。[詳細](/XSS.md)  |
|  [Tqlmap](https://github.com/epinna/tqlmap)  |テンプレートインジェクションの様々な組み合わせをすべて試してみることができる。  |
|  Knock  |Knockはワードリストに精度が左右される  |
|  DiscoverScript  |要調べ  |
|  Sublist3r  |検索エンジンを使用してサブドメインを列挙する。検索クエリを使用するため、ブラックリストに載ってしまう場合あり  |
|  SubBrute  |高い匿名性と高速スキャンを実現した。標的のネームサーバーにトラフィックを直接送信しない。<br>DNSレコードを列挙するDNSスパイダー機能も実行する（massDNSを使えば高い性能になる)  |
|  TruffleHog  |Gitのコミットりれきとブランチでエントロピーの高い文字列をスキャンして出力する。  |
|  Git-All-Secrets  |大きな組織を調べるときに使う。セットアップが少しめんどくさい。TruffleHogとrepo-supervisorを使ってスキャンを行う。  |
|  slurp  | バケットの列挙。キーワードまたはリストを受け取り複数の組み合わせを行い、パケットの検出を試みる。  |
|  BucketFinder  |パケットの特定と内容をすべてダウンロードして解析できるようにする。  |
|  [Spray](https://www.trustwave.com/en-us/resources/blogs/spiderlabs-blog/simplifying-password-spraying/)  |ブルートフォースアタックを行うツール？|
|  [ruler](https://github.com/sensepost/ruler)  |MAPI/HTTPまたはRPC/HTTPプロトコルを使ってExchangeサーバーとやり取りができる。 |
|  [Responder](https://github.com/lgandx/Responder)  |IPv6 / IPv4 LLMNR / NBT-NS/mDNSポイズナー？(要調べ)  |
|  Empire Powershell  |Powershellの機能を使って攻撃を再現する。かなり強力なツール(要調べ)  |
|  [Blood HoundAD](https://github.com/BloodHoundAD/BloodHound) |ActiveDirectory攻撃パスを継続的にマッピングおよび定量化する攻撃パス管理ソリューション？|
|  [CrackMapExec(CME)](https://github.com/byt3bl33d3r/CrackMapExec) |Active Direcotryへの自動セキュリティアセスメントツール(post-exploitation)で、できるだけIDS/IPSに検知されないように設計されたもの。<br>内部でImpacket, PowerSploit, Mimikittenzなどが使われているらしい。  |
|  [nikto](https://cirt.net/Nikto2)  |Webアプリケーション脆弱性スキャナー。かなり便利 |
|  [AutoRecon](https://github.com/Tib3rius/AutoRecon)  | TCPのデフォルト1000ポートスキャンのNmapScanを実行<br>そこからNmapのVulnスクリプトやNikto、enum4linuxなどを実行してくれる。空いてるポート見逃しが結構あるらしいので注意。[参考](https://kakyouim.hatenablog.com/entry/2020/04/17/182049#AutoRecon)  |
|  [LFI2RCE](https://github.com/takabaya-shi/LFI2RCE) |LFIなどの脆弱性に対して使う。  |




## 攻撃の手口
|  名前  |  説明  |
|  ----  |  ----  |
|  フィッシング  |受信者がドキュメントを開いたり、悪意のあるハイパーリンクにアクセスするように説得する電子メールなどを送信して、個人情報などを盗む。  |
|  スピアフィッシング  |成功率の高い攻撃の一種。特定の人を狙ってメールなどで攻撃をする。<br>ソーシャルエンジニアリングなどで人物の情報を収集することを中心としている。  |
|  プリテキスティング  |標的を説得して機密情報を露呈させたり、悪意のあるアクションを実行させる。電話や電子メールなども用いることが多い。  |
|  ベイティング  |戦略に則って、悪意のあるUSBなどを物理的なところに配置し、標的がそれを拾って内部システムに接続するように誘導すること。  |
|  XSS(クロスサイトスクリプティング) [詳細](/XSS.md)  |Webアプリケーションの脆弱性もしくはそれを利用した攻撃。<br>攻撃者がそこに悪質なサイトへ誘導するスクリプトを仕掛けることで、サイトに訪れるユーザーの個人情報などを詐取する。ブラウザによって動作が大きく異なる場合がある。<br>XSS作成参考:(https://github.com/foospidy/payloads/tree/master/other/xss)<br>(https://www.owasp.org/index.php/XSS_Filter_Evasion_Cheat_Sheet)  |
|  キーロガー  |キーボードから入力した文字情報などを記録するソフトウェアだが、悪用して個人情報などを盗むことも可能。  |
|  SQLインジェクション  |アプリケーションが想定しないSQL文を実行させることにより、データベースシステムを不正に操作する攻撃方法。[SQL MAP](http://sqlmap.org/)  |
|  NoSQLインジェクション  |SQL以外のデーターベースを標的にしたもの(※要調べ)<br>・[NoSQL injectionペイロード](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/NoSQL%20Injection)<br>・[Hacking NodeJS and MongoDB](https://blog.websecurify.com/2014/08/hacking-nodejs-and-mongodb.html)<br>・[Testing for NoSQL injection](https://www.owasp.org/index.php/Testing_for_NoSQL_injection) |
|  デシリアライゼーション攻撃  |データをシリアライズされた時と同じ状態に復元すること。このデシリアライゼーションの処理に対して、悪意のあるデータを与え、意図しないオブジェクトを復元させることで攻撃が成立する。  |
|  テンプレートエンジン攻撃  |ユーザー入力がテンプレートに直接渡され、テンプレートそのものが変更可能な時に起こる。<br>・[Server-Side Template Injection](http://blog.portswigger.net/2015/08/server-side-template-injection.html)<br>・[Yahoo! RCE via Spring Engine SSTI](https://hawkinsecurity.com/2017/12/13/rce-via-spring-engine-ssti/)<br>・[SSTI判別チートシート](https://raw.githubusercontent.com/swisskyrepo/PayloadsAllTheThings/master/Server%20Side%20Template%20Injection/Images/serverside.png) |
|  RCE(Remote Code Execution)  |オペレーティングシステムやWebアプリケーションの脆弱性を突いて任意のコードを実行するような攻撃手段。[チートシート](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/File%20Inclusion/README.md)  |
|  LFI(Local File Inclusion) |ターゲットのサーバ上のファイルに対し、不正なスクリプトを挿入し、デフォルトファイル名の変更、データのアップロードやダウンロードの実行等ができる  |
|  SSRF(Server-Side Request Forgery)  |通常の方法ではアクセスできないサーバーに対して攻撃を仕掛ける手法。・[localhostのエンコーディング](http://www.agarri.fr/docs/AppSecEU15-Server_side_browsing_considered_harmful.pdf)<br>・[Airbnbのバグバウンティ](https://buer.haus/2017/03/09/airbnb-chaining-third-party-open-redirect-into-server-side-request-forgery-ssrf-via-liveperson-chat/)  |
|  DOS(Denial of Attack)  | ウェブサービスを稼働しているサーバやネットワークなどのリソースに意図的に過剰な負荷をかけたり脆弱性をついたりすることでサービスを妨害すること  |
|  CSRF(クロスサイトリクエストフォージェリー)  |Webアプリケーションに存在する脆弱性、もしくはその脆弱性を利用した攻撃方法  |
|  XXE(XML External Entity) |XMLの外部参照機能を使って、機密情報を含む内部ファイルを読み出す不正行為。<br>・[Etienne StalmansのXXEペイロード](https://gist.github.com/staaldraad/01415b990939494879b4)<br>・[Daniel MiesslerのXXEペイロード](https://github.com/danielmiessler/SecLists/blob/master/Fuzzing/XXE-Fuzzing.txt)  |
|  ブルートフォースアタック  |可能な組合せを全て試すやり方  |
|  パスワードスプレー  |IDやパスワードを組み合わせて連続的に攻撃するブルートフォース攻撃の一種。アカウントロックを回避する手法を持つパスワード攻撃。  |
|  Null Byte攻撃  |「\0」「\x00」「%00」といった文字列の終わりを意味する制御文字をリクエストに含めることでセキュリティーチェックをすり抜ける手法。 |


## セキュリティ単語集etc...

|  名前  |  説明  |
|  ----  |  ----  |
| OWASP  |Webアプリケーションセキュリティの分野で自由に利用できる記事、方法論、ドキュメント、ツール、およびテクノロジを作成するオンラインコミュニティ。<br>https://owasp.org/www-chapter-japan/  |
|  スナップショット  |スナップショットとは、NAS上のファイルやフォルダの状態を定期的に記録・保存しておく技術。参考:(https://note.com/qnap/n/n2b9f5ff6bc11)  |  
|  C&Cサーバー(C2サーバー)  |侵入して乗っ取ったコンピュータを利用した攻撃で、踏み台のコンピュータを制御したり命令を出したりする。  |
|  BlackHat  |世界最大規模のセキュリティカンファレンス。  |
|  SSTI  |Server-Side Template Injection  |
|  フォレンジック  |デジタルデバイスに記録された情報の回収と分析調査などを行うこと  |
|  XML(Extensible Markup Language)  |データを読みやすい形式で送信/格納することを目的として設計された  |
|  DTD(Document Type Declaration)  |SGMLやXML、HTMLなどのマークアップ言語で記述された文書の冒頭などに記載される。  |
|  MAPI(Messaging Application Programming Interface )/HTTP  |Outlook と Exchange の接続の信頼性と安定性を改善するために、<br>トランスポート層を業界標準の HTTP モデルに移行させているトランスポート プロトコル。  |
|  RPC/HTTP  |Microsoft Outlook クライアントが HTTP を介して Microsoft Exchange サーバーにアクセスするための Microsoft プロトコル。  |
|  メモリリーク  |プログラミングにおけるバグの一種。プログラムが確保したメモリの一部、または全部を解放するのを忘れ、確保したままになってしまうこと。|
|  SaaS  |必要な機能を必要な分だけサービスとして利用できるようにしたソフトウェアもしくはその提供形態のこと。  |
|  NTLM(NT LAN Manager)  |マイクロソフトによるセキュリティプロトコル。LAN Manager (LANMAN, LM) の後継。  |
|  Activate Directory |ディレクトリ・サービス・システム。ユーザとコンピュータリソースを管理するコンポーネント群の総称  |


