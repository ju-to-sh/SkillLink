### ■ サービス概要
タイピングとRuby/Railsの学習が１つのサイトでできるRuby/Rails特化の学習サービスです。学習→タイピングを繰り返すことで、知識定着＆タイピング速度UPができます。

### ■ このサービスへの思い・作りたい理由

プログラミング学習中、開発スピードを上げるためタイピング速度をより早くしたいと考えていましたが、知識習得に時間を割くことを優先しがちで、継続してタイピング練習に取り組むことができませんでした。<br>
そのため、知識習得とタイピング練習がまとめてできれば、片方を疎かにせずに継続的に取り組めるかつ楽しく学習できるのではと考えました。

### ■ ユーザー層について
対象ユーザー層：<br>
Ruby/Railsの初学者で、学習しながらタイピング速度を向上させたい方<br>
理由：<br>
①タイピング速度が遅いプログラミング初学者にとって、学習しながらタイピング速度を向上させるサイトがあれば需要があると考えたため<br>
②学習した内容をアウトプットする時に、タイピング練習が同時に行えれば効率的だと考えたため

### ■ サービスの利用イメージ
**【利用イメージ】**<br>

学習したい内容（Ruby/Railsに特化）について、タイピングとクイズゲームを通してタイピング速度の向上と理解度チェックを図ります。<br>
また、学習記録を管理でき、ゲーム実績はランキング形式とし、ユーザー同士で実績をシェアできます。<br>

**【使用画面の詳細】**<br>
| トップページ  | ゲーム選択ページ |
| ------------- | ------------- |
| [![Image from Gyazo](https://i.gyazo.com/1d5fb5ffa014b323bac360dbc3becda4.png)](https://gyazo.com/1d5fb5ffa014b323bac360dbc3becda4)  | [![Image from Gyazo](https://i.gyazo.com/59f5dcc32217f8ad6a46916d981cb5db.png)](https://gyazo.com/59f5dcc32217f8ad6a46916d981cb5db) |
| サービス概要の説明および問題を解くボタンを押すことで、ゲーム選択画面へ遷移する。  | クイズゲームかタイピングゲームを選択できる。ログインなしでもプレイ可能であり、ログインしてプレイした場合は、学習記録として結果が残る。  |

| クイズ一覧ページ  | タイピング一覧ページ |
| ------------- | ------------- |
| [![Image from Gyazo](https://i.gyazo.com/662d7d54c60c980d7cd6c3069125f6de.png)](https://gyazo.com/662d7d54c60c980d7cd6c3069125f6de)  | [![Image from Gyazo](https://i.gyazo.com/55766a63ff28184509f0b5352b971560.png)](https://gyazo.com/55766a63ff28184509f0b5352b971560)  |
| 4クイズにはカテゴリー（Ruby or Rails）、レベルの表示あり  | クイズ同様、カテゴリー（Ruby or Rails）、レベルの表示あり |

| ランキング一覧ページ  | 問題検索ページ |
| ------------- | ------------- |
| [![Image from Gyazo](https://i.gyazo.com/67990ed7cee4d83b722e12d4a66bb4de.gif)](https://gyazo.com/67990ed7cee4d83b722e12d4a66bb4de)  | [![Image from Gyazo](https://i.gyazo.com/220dc5ebb1c60d2e670df356cb1ec03c.gif)](https://gyazo.com/220dc5ebb1c60d2e670df356cb1ec03c)  |
| 会員登録したユーザーのタイピング結果をランキングとして表示。タイプ速度とミスタイプ数からスコアを算出しているため、速くてミスタイプが少ないほどスコアが高くなる。  | タイトル名、カテゴリー、レベルで問題を検索することができる。  |

| クイズゲームページ  | クイズ結果ページ |
| ------------- | ------------- |
| [![Image from Gyazo](https://i.gyazo.com/791411e67eb5c26181ca2c80f5441982.gif)](https://gyazo.com/791411e67eb5c26181ca2c80f5441982)  | [![Image from Gyazo](https://i.gyazo.com/b05adca59b2e262805f783ef08872e8d.gif)](https://gyazo.com/b05adca59b2e262805f783ef08872e8d)  |
| 4択クイズで1つのクイズにつき5問出題される。何問目を解いているか把握できるように、画面上部にステッパーを表示。  | 正解数と各クイズの回答およびユーザー回答を表示。画面下部のボタンより問題一覧画面に遷移する。 |

| タイピングゲームページ  | タイピング結果（モーダル） |
| ------------- | ------------- |
| [![Image from Gyazo](https://i.gyazo.com/f8068a80aa732db63d33f660b7519ef1.gif)](https://gyazo.com/f8068a80aa732db63d33f660b7519ef1)  | [![Image from Gyazo](https://i.gyazo.com/20d8262ea9bdb281aabdc30e9da7635c.gif)](https://gyazo.com/20d8262ea9bdb281aabdc30e9da7635c) |
| 1つのタイピング問題につき5問出題される。入力対象文字の場合：背景色グレー＋黒字、正しい入力の場合：緑字、誤入力：赤字で表示。  | タイピング結果をモーダルで表示。表示内容は、タイピング速度、ミスタイプ回数、スコアの3項目。  |

| X投稿機能  | 学習記録ページ |
| ------------- | ------------- |
| [![Image from Gyazo](https://i.gyazo.com/063c1a52f0794c0decff5daa90e3707d.gif)](https://gyazo.com/063c1a52f0794c0decff5daa90e3707d)  | [![Image from Gyazo](https://i.gyazo.com/ded702c30283a361dbe5cd19b1f2de55.gif)](https://gyazo.com/ded702c30283a361dbe5cd19b1f2de55)  |
| タイピング結果を容易にXでシェアできるように投稿ボタンを設置。ボタンを押下後、Xの投稿内容にタイピング結果とアプリのリンク先をあらかじめ表示する。  | ログイン状態でクイズorタイピング問題を解くことで、カレンダーに解いた問題数の実績を表示する。また、タイピングの場合はグラフで過去実績のトレンドを把握することができる。  |

| お気に入り機能  | マイページ |
| ------------- | ------------- |
| [![Image from Gyazo](https://i.gyazo.com/e159de411861af94ca1dcf6743b5cd81.gif)](https://gyazo.com/e159de411861af94ca1dcf6743b5cd81)  | [![Image from Gyazo](https://i.gyazo.com/67b589d4d28d56b853483d316ffa214f.gif)](https://gyazo.com/67b589d4d28d56b853483d316ffa214f)  |
| ログイン状態の場合、各クイズ問題にお気に入りボタンが表示される。お気に入りした問題については、ヘッダー上部のお気に入り一覧から画面遷移することで、容易に問題にアクセスすることができる。  | ログイン状態の場合、ユーザー情報を表示するマイページに遷移することができる。ニックネームやユーザーアイコンの編集などができる。  |

**【得られるもの】**
- Ruby/Railsの基礎的な知識
- タイピング速度の向上

### ■ サービスの差別化ポイント・推しポイント
**【競合するサービス】**<br>
- [Codedrill](https://www.code-drill.com/chars/typing/type_Ruby)：Rubyのタイピングゲーム

**【差別化ポイントと優位点】**<br>
- RubyとRails両方を学習しながらタイピング練習できる点
- タイピングとクイズを併用することで効率的に知識のレベルUP＆タイピング速度UPができる点
- 学習記録を管理できる点
- ゲーム実績をユーザーとシェアできる点

### ■ 機能
- ログイン機能
- 検索機能
- プロフィール画像投稿機能
- タイピング練習機能
- クイズ機能
- 学習記録管理機能（カレンダー表示/グラフ）
- Xへの投稿機能
- ランキング表示機能
- お気に入り機能
- パスワードリセット機能

### ■ 使用技術一覧
フロントエンド：React、Typescript<br>
  - CSSフレームワーク: Material UI
  - 状態管理ライブラリ：Recoil

バックエンド：Ruby、Ruby on Rails<br>
  - コード解析 / フォーマッター: Rubocop
  - テストフレームワーク: RSpec

データベース：PostgreSQL<br>
インフラ：herokuおよびvercel,AWS S3<br>
開発環境：Doker/Docker-compose<br>
CI/CD：Github Actions

### ■ 画面遷移図/UI
Figma：<br>
画面遷移図
https://www.figma.com/design/miSHjWP3PXquC20SsSSM3U/%E7%94%BB%E9%9D%A2%E8%A8%AD%E8%A8%88?node-id=8%3A299&t=enpz9Xjdo2IGsoee-1<br>
UI
https://www.figma.com/design/miSHjWP3PXquC20SsSSM3U/%E7%94%BB%E9%9D%A2%E8%A8%AD%E8%A8%88?node-id=26%3A650&t=4ielewCafDRu9tic-1

### ■ ER図
[![Image from Gyazo](https://i.gyazo.com/d19908e9307c257223a3888133a873b6.png)](https://gyazo.com/d19908e9307c257223a3888133a873b6)

