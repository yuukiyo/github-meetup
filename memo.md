# 8/2 11:30 - 13:30 GitHub MeetUp
### GitHub堀江さんから挨拶
* SNSの拡散とかしないでね
* ピザと寿司あとで来るよ

### Cyber Agent
* Amebaのinfraを支えるGHEとアレコレ
* 岩永 翔 kakerukaeru
- AmebaとGHE
- AmebaとInfra
  - 2004年から発足なので以外と長い
  - private cloud(openstack + kvm) + AWS + GCP
  - public cloudは把握できていない
  - インフラエンジニアは20人くらい
  - インフラやばい
- Amebaのinfraを支えるGHEとアレコレ
  - CI/CDを加速させるGitHub Integration達
  - OS ImageのCI/CD
  - GHE CCI packer serverspec
  - GHE CCI terraform
  - GHE CCI serverspec chef
  - GHE jenkins roadworker
  - hubotにbranchをきらせる？
    - なんでだろ。
- まとめ
  - GHEを導入してinfraのCode化が加速
  - 豊富なIntegrationのおかげでCI/CD化が楽に出来た

### LINE
* LINEでのGHE
* 石島秀晃 2011/10入社
* 会社の成長に伴う運用対応
* 2012年から利用を開始
* LINEのソース全てGHEで管理
* LFS
  - 今後サポート予定
* スペック
  - 今後サポート予定
  - ssd 10Gbps iSCSI
  - メモリ96GB
* 正社員用のGHEと協力会社 + 正社員用GHEで分けた
  - 運用コストが2倍
  - 複数のGHEをもつ。。。
  - 1Jenkinsに対して2GHEができなくて困った
* GHEへのお願い
  - 権限追加してほしい
    - public
    - protected:認証必要（正社員のみ）
    - private
  - adminAPIを増やして欲しい

### Recruit Life Style
* 宮井康宏 GitHub:mia-0032
* Drone使ってる
* Droneからのpacker terraform ansible serverspec使ってる

### KDDI

### Cookpad
* 2012年から使ってる
* AWS r3.xlarge 500GB gp2
* AWS r3.xlarge 500GB gp2
* Zatsu repoが斬新だった
  - 深夜の飲み会とかで思いついたやつとかがある

### Nikkei
 * 紙面ビューアーの内製とGithub
 * 猪飼 ikai taishi
 * 内製の背景
   - 短いサイクルでのリリースの重要性
   - ユーザーにとっての価値とは？
   - 3年前に外注したアプリはあった
* アプリがクラッシュしたらお客様投稿フォームを表示してデータをためてる
  - AppStoreに飛ばすとネガティブなこと書かれちゃうので

### GitHub
* TAKAFUMI IKEDA@IKEIKE443
* GHE:2.7
  - 15:00くらいに出そう
  - 2.7をもって、2.2はサポート対象外
  - ワークフロー
    - コミットに対してGPG署名可能
    - Issue/PRのコメントが編集されたことがわかるように
      - editedって文字が出る
    - Issue/PRの複数アサイン可能
    - タスクリストの入れ替え
    - 長過ぎIssueのレンダリング工夫
    - CloneのUIを変更
    - モバイル版のヘッダー改善
  - plattform
    - webhookイベント追加
    - リアクションAPI
    - IssueロックAPI
    - Pull RequestマージAPI
      - 2.6のSquashMergeにするかをAPIにて選択できるようになった
    - Pre-receive API
    - Email通知の改善
    - ProtectedBranchAPIの破壊的改善
  - ユーザープロフィール関連
    - リポジトリ一覧のカスタマイズ
      - 順番入れ替えできるようになった
    - Privateコントリビューションの表示
    - UserBio
  - Git2.9
