### ■サービス概要
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

### ■サービスの利用イメージ
**【利用イメージ】**<br>

学習したい内容（Ruby/Railsに特化）について、タイピングとクイズゲームを通してタイピング速度の向上と理解度チェックを図ります。<br>
また、学習記録を管理でき、ゲーム実績はランキング形式とし、ユーザー同士で実績をシェアできます。<br>
タイピングとクイズゲームについて具体的な内容は以下の通りです。<br>
<u>タイピングゲーム</u><br>
使用頻度の高いメソッド名（ifやmapなど）とそのメソッドで出来ること・使用例をタイピング問題として出題します。以下は一例です。
```
ifは条件式を評価した結果が真である時、then 以下の式を評価します。 if の条件式が偽であれば elsif の条件を評価します。
```

```
if age >= 12 then
  print "adult fee\n"
else
  print "child fee\n"
end
gender = if foo.gender == "male" then "male" else "female" end
```

<u>クイズゲーム</u><br>
4択のクイズで１つの選択肢を選んで回答するクイズにすることを考えています。クイズ内容のイメージは、RUNTEQの基礎STEP総復習クイズのような理解できていないと初学者が引っ掛かりそうな内容を中心に出題します。また、クイズ結果画面では正解数に加え、クイズの解説を入れる想定です。


**【得られるもの】**
- Ruby/Railsの基礎的な知識
- タイピング速度の向上

### ■ ユーザーの獲得について
Ruby/Railsの初学者でタイピング速度を早くしたいユーザーに対して、学習とタイピング練習を効率的に実施できることをアピールする。

### ■ サービスの差別化ポイント・推しポイント
**【競合するサービス】**<br>
- [Codedrill](https://www.code-drill.com/chars/typing/type_Ruby)：Rubyのタイピングゲーム

**【差別化ポイントと優位点】**<br>
- RubyとRails両方を学習しながらタイピング練習できる点
- タイピングとクイズを併用することで効率的に知識のレベルUP＆タイピング速度UPができる点
- 学習記録を管理できる点
- ゲーム実績をユーザーとシェアできる点

### ■ 機能候補
**【MVPリリース時】**<br>
- ログイン機能
- ゲストログイン機能
- 検索機能
- プロフィール画像投稿機能
- タイピング練習機能
- クイズ機能
- 学習記録管理機能
- ユーザーのCRUD機能
- Xへの投稿機能
- ランキング表示機能
- お気に入り機能

**【本リリース時】**<br>
- タイピング実績のグラフ化
- 管理者画面
- CSVインポート・エクスポート機能


### ■ 機能の実装方針予定
フロントエンドに関しては、過去にチーム開発でReact,Reduxでの開発経験があるため、作成初期から実装したいと考えております。
Typescriptについては、キャッチアップが不十分なためMVPリリース後にキャチアップを予定しています。
#### 使用予定技術一覧
フロントエンド：React、Typescript<br>
  - コード解析 / フォーマッター: ESlint&prettier
  - CSSフレームワーク: Tailwind CSS
  - 状態管理ライブラリ：Redux

バックエンド：Ruby、Ruby on Rails<br>
  - コード解析 / フォーマッター: Rubocop
  - テストフレームワーク: RSpec

データベース：Mysql<br>
インフラ：AWS/Nginx/Unicorn/Mysql<br>
開発環境：Doker/Docker-compose<br>
認証：OAuth 2.0

実装予定の機能については、以下のような技術等を使用する想定です。（CRUD機能で実装できるものは割愛）

- ログイン/ゲストログイン機能<br>
Sorcery, OAuth 2.0
- 検索機能<br>
ransack
- プロフィール画像投稿機能<br>
carrierwave＆mini_magick
- タイピング練習機能<br>
Material Tailwind
- クイズ機能<br>
Material Tailwind
- タイピング実績のグラフ化<br>
chartkick
- 管理者画面<br>
Active Adimin
- CSVインポート・エクスポート機能<br>
 activerecord-import
