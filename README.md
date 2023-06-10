# team-a-devlog

### 要件定義
- 目的
  - ウェブアプリケーションとしてのカードゲーム実装を優先し、モバイルやデスクトップアプリとしてのデプロイを目標とする。
- 機能要件
  - easy, medium, hardの3つの難易度で、敵のCPUと対戦できること
  - ルール、勝利条件、プレイヤー数が異なる複数のトランプゲームモードに対応すること
対応するゲームモード：ブラックジャック（2-7人）、ウォー（2人）、スピード（2人）、ポーカー
各プレイヤーがゲームに参加するために満たさなければならない最低入札要件があるゲーム。もしプレイヤーが最低入札額を満たすことができなければ、ゲームに負けることになります。：ブラックジャック、ポーカー、テキサスホールデム
点数制のゲームで、最も高い点数を獲得した人が勝者となるゲーム：ラミー、戦争、スピード
  - ユーザーの手が有効かどうかをチェックするバリデーションがあること
  - 各ゲームモードに、ユーザーがゲームのプレイ方法を学ぶことができる簡単なチュートリアルがあること
 各ゲームモードに、ユーザーがゲームのルールを理解するためのチートシートメニューがあること
  - Webアプリへのリンク、またはアプリの最新バージョンをダウンロードできるホームページを用意すること
- 非機能要件
  - コードベースが、将来的にトランプゲームのモードを簡単に追加できるように拡張可能な状態になっていること
  - アプリは、ユーザーにとってシンプルでわかりやすく感じられ、混乱や遅延なく効果的に使い始めることができること
  - ソフトウェアが、クロスプラットフォームであること。ウェブアプリ（ブラウザ）としてアクセスできるほか、デスクトップアプリ（Windows、Linux、Mac）、モバイルアプリ（iOS、Android）としてダウンロードすることができること。
  - インストールするデバイスやオペレーティングシステムの種類にかかわらず、ソフトウェアのインストールプロセスがシンプルで効率的であること。これにより、ソフトウェアはすべてのプラットフォームで簡単かつ迅速にインストールできるようになります。

  - ユーザーがソフトウェアをダウンロードできるページには、常に最新のバージョンがダウンロード可能でなければならないこと。

  - ソフトウェアのデザインとユーザーインターフェースが最新で視覚的に魅力的であること。

### 議事録
#### 5/27
#### やったこと
- タスク管理の手段を決定
  - GitHub Issues
- 技術スタックの選定
  - Platform: Web, Desktop, Mobile
  - Architecture: MVC
  - Frontend: TypeScript + Phaser
  - Backend: Node.js web server
  - Storage: Local Storage
  - Language: Javascript
  - Frameworks & Tools: Phaser Game Framework, Apache Cordova

#### 課題
- GitHub Actions, eslint
- deploy環境の選定
  - Vercel、Netlify など

#### 5/30
#### やりたいこと
- コーディング規約
- GitHubルール
- テスト計画
- クラス図、アクテビティ図
- デプロイ環境の選定
- フロントエンドフレームワークについて

#### やってきたこと
- eslint、prettierを導入し、コードのフォーマットを可能にした。
- huskyを導入し、コミットの際に自動的にコードがフォーマットされるようにした。
- 技術スタック構成図を作成した。
- ワイヤーフレームを作成した。

#### やったこと
- コーディング規約の決定。原則[AirBnb](https://mitsuruog.github.io/javascript-style-guide/)に則る。
- [GitHubのルール](https://suwaru.tokyo/%E3%80%90%E5%BF%85%E9%A0%88%E3%80%91git%E3%82%B3%E3%83%9F%E3%83%83%E3%83%88%E3%81%AE%E6%9B%B8%E3%81%8D%E6%96%B9%E3%83%BB%E4%BD%9C%E6%B3%95%E3%80%90prefix-emoji%E3%80%91/)
  - Git flow
  - ブランチ名のプレフィクス
  - issueへのリンク

#### 直面した問題
- huskyによるコミットの際のコードフォーマットが機能しなかった。
pre-commitの実行権限が制限されていたので、実行権限を変更して解決

### 課題
- プルリクのテンプレートを作成
- クラス図、アクテビティ図
- プロトタイプの作成 (Phaserの調査)
- デプロイ環境の調査 (Vercel, Netlify, Heroku, etc.)
  - 利便性、価格
- フロントエンドフレームワークの調査 (React, Next.js)
- Tailwind CSSの調査
- スプリントの計画
- テストツールの選定、導入

#### 6/3
#### やりたいこと
- 各自が調べてきた内容の共有
- ディレクトリ構造の決定
- 最低限の環境構築
- 採用するフレームワーク、ライブラリ、ホスティング環境の決定
- 次週のスプリント計画
- カードの表示 (画像、CSS？)
- アセットの見繕い
- 次のミーティング日程

#### やってきたこと
- Phaserの調査、プロトタイプの作成

#### やったこと
- カードの表示はとりあえず画像
- 採用するフレームワーク、ライブラリ、ホスティング環境の決定
    - フレームワーク、ライブラリ
        - Next.js
        - React.js
        - Phaser.js
        - tailwindCSS
    - CI/CD
        - husky
        - eslint
        - prettier
    - ホスティング環境
        - Vercel
    - 保留
        - データベース
- 次週のスプリント計画
   - 下記
- 次のミーティング日程
    - 6/6火曜日10:00
    - 6/10土曜日10:00

#### 直面した問題
- husky

### 課題
- 環境構築　(ディレクトリ構造の決定) 6/4
- husky 6/5
- クラス図の見直し 6/5
- アセットの見繕い 6/5
- Next.jsの学習 6/5
- ワイヤーフレームの充実 6/5
- 基本的な画面遷移 6/9
- クラス作成 6/9

#### 6/9
#### やりたいこと
- 各自が調べてきた内容の共有
- ログイン機能実装するか

#### やってきたこと
- [アセットの見繕い](https://github.com/recursion-team-a/card-games/issues/22)
- [ワイヤーフレームワークの充実](https://github.com/recursion-team-a/card-games/issues/21)
- [環境構築　(ディレクトリ構造の決定)](https://github.com/recursion-team-a/card-games/issues/18)
- [huskyによるコミット時のコードフォーマット](https://github.com/recursion-team-a/card-games/issues/19)
- [クラス図の見直し](https://github.com/recursion-team-a/card-games/issues/20)

#### やったこと
- [アセットの見繕い](https://github.com/recursion-team-a/card-games/issues/22)
- ログイン機能は実装する (予定)
- ディレクトリ構造
```
- src
    -app
    - components
    - model
          - common
          - BlackJack
          - War
          - Speed
          - etc.
```

#### 直面した問題
- husky

### 課題
- 基本的な画面遷移 6/9
- クラス作成 6/9
    - table
    - player
- jestの調査 6/9

#### 6/10
#### やりたいこと
- やってきたことの共有
- 次回のミーティングまでにすること
- eslintとコーディング規約
- jest
- 日程
- ファイル名の命名

#### やってきたこと
- 基本クラスの作成
- ファイル名 e.g. 'ExampleClass.ts'
- ディレクトリ名 e.g. 'exampleDirectory'

#### やったこと
- 次回の日程
  - 水曜日　14:00-16:00
  - 土曜日 10:00-12:00
- 各自のタスク進捗状況を共有
- jestについての計画

#### 直面した問題
- [Next.jsとPhaser.jsの連携](https://github.com/recursion-team-a/card-games/issues#:~:text=1-,%E5%9F%BA%E6%9C%AC%E7%9A%84%E3%81%AA%E7%94%BB%E9%9D%A2%E9%81%B7%E7%A7%BB%206/9,-%2323%20opened%20last)
- Tableクラス実装の続き

### 課題
今週の目標
ゲームとして最低限動かせる形

- Tableクラスの実装 K
- Phaser、Nextの連携 T
- Playerクラスの修正 H
- eslintとコーディング規約 K
- jestの導入 T
