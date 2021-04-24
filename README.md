# 職務経歴書

## 職務経歴

### 株式会社ドワンゴ(2016/4~)

大学受験やプログラミングなど様々なコンテンツで学習できるアプリケーションを開発。
プロジェクト内で 3 つのポジションを経験している。

- 2016 年〜2019 年 Android アプリ開発
- 2019 年〜2020 年 スマートフォンアプリグループリーダー
- 2021 年 フロントエンドセクションマネージャー

#### Android アプリ開発

アプリ立ち上げ後に参画。

最初は Android 初心者から始まる。
経験を積むにつれて、徐々にコアメンバー・唯一のフルコミット開発者となる。
アプリ立ち上げ時の技術的負債が大きく、その負債と戦いながらいかにモダンな技術を取り入れていくかが課題であった。

##### Kotlin 導入

プライベートで利用してとても快適だったことから、 Android 公式言語になる以前の 2017 年 に Kotlin を導入した。
null 安全性や、 RxJava をはじめとするラムダ式の記述の簡潔さ、data class によるモデル記述といった多くのメリットを得ることができた。
Kotlin のコード規約の和訳などを通して、Kotlin の利用方法をチームに周知した。
今となっては Kotlin は Android 公式言語となり、 Android 開発のデファクトスタンダードとなったためよい選択だった。
導入後は、開発で着手したところを改修する方針で少しずつ移行を進めた。
私がメインのコミッターであるときには完遂できなかったが、他メンバーが引き継いでくれたことで完了した。

##### アーキテクチャの刷新

MVP ながらも Presenter に全てのロジックが集中する Fat Presenter になってしまっていた。
既存のアーキテクチャからの移行のしやすさも勘案した RxJava を利用した MVVM 風の独自アーキテクチャに更新した。
（当時はまだ Android Architecture Component がなかった）。
このアーキテクチャによって、Fat Presenter に集中していたロジックを個別のテスタブルなファイルに切り出すことが可能となった。
テストがついていない 1000 行を超えるファイルを解体し、テスト付きのロジックとして切り出した。
ロジックが切り出されたことで、見積もりの際にもロジック=作業単位=PR 単位として切り出すことが可能となり、見積もりもしやすくなった。
導入後は、開発で着手したところを改修する方針で少しずつ移行を進めた。
こちらも私がメインのコミッターであるときには完遂できなかったが、他メンバーが引き継いでくれたことで完了した。

##### CI/CD の整備

もともと Jenkins による CI/CD を行っていたが、 Bitrise に移行した。

また、メンバーの 1 名が途中から昇進して多忙になりコードレビューのみ行ってもらう体制になった。
その際にも PR 単位でアプリ配信を行い、レビュー時の動作確認をより簡単にしてもらえるような体制を作った。

#### スマートフォングループリーダー

iOS も含めたスマートフォングループのリーダーに任命された。

##### iOS キャッチアップ

業務に加えてプライベートでも iOS アプリを試作し、iOS アプリ作成の大まかな概要を掴んだ。
iOS は RxSwift を用いて開発していたため、Android の Rx 経験を活かしてレビューできた。

ビルドやリリース作業などの工程を経験し、iOS に関してもサポート程度であれば可能なスキルを身に着けた。

##### プロジェクト管理

スマートフォンアプリ視点での要件定義・見積もり・工程管理に携わった。

iOS チームにはフルタイムの社員がリーダーの私しかいなかった。
スマートフォンの要件を iOS メンバーと相談しながら決め、タスクに落とし込む必要があった。
工数と実装要件のバランスがとれるよう注意を払った。

また、iOS アプリのマネジメントを通じて他の人に任せるということを経験できた。
Android アプリと異なり、 iOS は自分が隅々まで知らないので勝手がわかっていなかった。

#### フロントエンドマネージャー

PC も含めたフロントエンドセクションのマネージャーに任命された。

##### なんでもやる

組織改編など様々な事情によりマネジメントレイヤーの人員が半分以上入れ替わった。
そんな中で、マネージャーとして必要と思われることはなんでも取り組んだ。
そこでは、自分が潰れないように相談窓口を確保することに気をつけた。
上位レイヤーとの接点を積極的に増やし、随時問題を共有しながら解決した。

##### QA チームの新設

それまで開発者が手弁当でテストを行っていた。
しかし、担当者によってテスト実施方法やクオリティがまちまちになってしまう問題があった。
QA チームの新設によって横串で品質を保証できる組織体制を作っている。

##### タイムマネジメント

マネージャーとなって参加するミーティングが増えた。
意図しなければ作業時間を確保できなくなった。
自身の作業時間は自分だけでなく全体の効率的な組織運営を考える上で非常に重要である。
不要なミーティングを減らし、束ねることで時間を意図的に確保する習慣を身に着けた。

### 株式会社チアドライブ(2021/12~)

車の運転を支援するアプリの開発。
React Native を利用したクロスプラットフォームアプリである。
リリース前のタイミングで Android 固有の問題を主に担当するエンジニアとして参画。

#### 参画思想

月ごとの作業が約 20 時間、作業時間帯は不定期である。
この環境を鑑みて、以下を意識して立ち回っている。

- レバレッジの効く作業
- 他の人をブロックしない作業

限られた時間では、どうしても各機能実装のような作業でバリューを出すのは難しい。
それよりも、チーム全体の作業効率を高めるようなレバレッジの効く作業に意識して取り組んでいる。

また、作業時間もバラバラのため、自分が作業のブロック要因になると全体が止まってしまう。
Android 固有の問題でリリースできないなどあれば優先的に対応している。

#### CI/CD の整備

プロジェクト参画当初は、そもそも Android でビルドできないという状況になってしまっていた。
それを修正するのは当たり前として、再発防止策として Bitrise と fastlane を用いた CI 環境を整え、PR の段階で検知するようにした。

#### lint/format の整備

個人的にも不慣れな JavaScript で書かれているため、コードの妥当性を担保するために lint/format を整備した。
Huskey を使って eslint/prettier をコミット時に自動で走らせるようにした。
また、Danger で eslint のエラーを PR にコメントする設定を追加した。

## スキル

### Android 開発

| 種別           | 詳細                                                   |
| :------------- | :----------------------------------------------------- |
| 言語           | Kotlin, Java                                           |
| ライブラリ     | Jetpack, RxJava, OkHttp, Glide, Mockito                |
| アーキテクチャ | クリーンアーキテクチャをベースにした独自アーキテクチャ |
| CI/CD          | Bitrise, Jenkins, DeployGate                           |

### ツール

| 種別                 | 詳細                                                                |
| :------------------- | :------------------------------------------------------------------ |
| バージョン管理       | git                                                                 |
| チーム開発           | GitHub. PR とレビューに基づく開発                                   |
| タスク管理           | JIRA                                                                |
| ドキュメンテーション | Confluence, Google Docs, Spreadsheet                                |
| コミュニケーション   | Slack ( Slack Bot の作成と運用による業務効率化を含む）, Google Meet |

### 資格

- 基本情報技術者資格
- 応用情報技術者資格

## アウトプット

https://qiita.com/hmiyado
