# Laratime
# 推しアイデア
自分の予定を入れるのではなく、暇な時間を入れるという逆転発想
# 作った背景
友達に空いてる時間を聞くのはめんどくさい...
だから
空いてる時間を入力して共有しよう！

# 推し技術
・手軽に入力
・グループごとに予定を分けることができる
・fullcalendarでカレンダーを表示
・deployに挑戦

# 役割分担
安藤：グループ関係
柳井：fullcalendar azureでデプロイ
首藤：db ルーティング
# プロジェクト概要

![image](https://ptera-publish.topaz.dev/project/01GG16N32XPZ1EYSKRE6MNGD67.png)
## グループ作成
グループid・パスワードを設定し、グループを作成する。
![image](https://ptera-publish.topaz.dev/project/01GG16KN79H9H43P6NP0Z9AFEK.png)

##  グループ参加
グループid・パスワードを入力し、グループに参加
![image](https://ptera-publish.topaz.dev/project/01GG16P8WGFEBX92SZ3E6DPBDB.png)

##  カレンダーページ
カレンダーをクリックすることで予定のタイトルを入力することができ、予定を追加できる。作成された予定をドラッグすることで予定の時間を変更することができる。 イベントをクリックすることで予定の詳細を閲覧することができる。
![image](https://ptera-publish.topaz.dev/project/01GG16GXJEWYRBT3MS4P2S57QW.png)


# アーキテクチャ図
![image](https://ptera-publish.topaz.dev/project/01GG162WP32CAM52ZV23XJTGXD.png)

![image](https://ptera-publish.topaz.dev/project/01GG162MX1FE66V8BX2A2XXX76.png)

![image](https://ptera-publish.topaz.dev/project/01GG124EZ7CAM187D9BPRWQENX.png)
# 技術的チャレンジ

## fullcalendarをcdnからnpmに
参考サイトがcdnにやっていたため、npmでfullcalendarを導入
cdn
![image](https://ptera-publish.topaz.dev/project/01GG1494548DZEZ8N49W7G543T.png)
npm
![image](https://ptera-publish.topaz.dev/project/01GG124EZ7CAM187D9BPRWQENX.png)
## azureを使ってデプロイ
![image](https://ptera-publish.topaz.dev/project/01GG122DR22Z95TTQ94PPYBXT3.png)

![image](https://ptera-publish.topaz.dev/project/01GG16H2PTZA3WZE08ZJ38T9W9.png)
index画面しか表示されず、他の画面はエラーがでていたが、npm install npm run buildで解決した
![image](https://ptera-publish.topaz.dev/project/01GG124EZ7CAM187D9BPRWQENX.png)
※localのようには動かない
github
https://github.com/Yanai1005/phase2_teamC

# チーム開発での問題/難しかった事と克服した事と反省点

・githubの扱いがわからずpush -fしてを上書きしていた（首藤）
  役割分担をはっきりさせて、同じファイルに同時に記述する状況を減らして、conflictを減らした。
  反省点  テーブルを変更するときに意思疎通が取れず問題が発生したこと
・コミュニケーションが不足（柳井）
  可能な限り、会議をして、コミュニケーションをとった
  反省点  チーム開発ようにgithubアカウントを作るべきだった
・（安藤）


