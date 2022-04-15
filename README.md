# セキュリティノート

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



## 攻撃の手口
|  名前  |  説明  |
|  ----  |  ----  |
|  スピアフィッシング  |成功率の高い攻撃の一種。特定の人を狙ってメールなどで攻撃をする。<br>ソーシャルエンジニアリングなどで人物の情報を収集することを中心としている。  |


