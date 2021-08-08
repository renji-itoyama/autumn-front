# autumn-front 

### ＜大前提として、エンジニアたる者はインストールしておきたいもの＞
※今回使わないとしても、後々役に立ったりするので入れておいてください。
- [Homebrew](https://brew.sh/)のインストール<br>
  Homebrewは、言語やフレームワーク、パッケージなど色々インストールする際に自分のPCを汚さないためのものです。
- dockerのインストール<br>
  もちろん[公式サイト](https://docs.docker.com/)からダウンロードも可能ですが、せっかくbrewを入れたのでbrewを使ってインストールしましょう。<br>
  `$ brew install --cask docker`
  
- 上記に加え、少し作業は多いですが[こちら](https://qiita.com/newt0/items/80164665e7e83ec7a669)もおすすめです。<br>
  ❗️ **「開発環境構築」** のエリアはやらない方が賢明です。
  
<br>
<br>

## ＜仮想環境の構築手順＞

### ① Anacondaのインストール
[こちらのリンク](https://www.anaconda.com/products/individual#Downloads)から、OSに合うものをインストールしてください。

**❗️ここから先は、「ターミナル（MAC）」または「コマンドプロンプト（Windows）」を起動して行ってください**

### ②condaコマンドを使って仮想環境の構築
ターミナルで以下のコマンドを実行してください。<br>
`$ conda create -n autumn-front`

### ③仮想環境に入る
`$ conda activate autumn-front`

---

#### 〜Anacondaに関する予備知識〜

仮想環境に入ると、ターミナルの表記が`UserNamenoMacBook-Pro: UserName$`から<br>
`(autumn-front)UserNamenoMacBook-Pro: UserName$`と表記が変わります。<br>
この状態になっていればAnaconda（仮想環境）に入れている証拠です。<br>
<br>
仮想環境から抜けたい場合は、`conda deactivate`と打てば抜けられます。<br>
もし抜けずに`(base)UserNamenoMacBook-Pro: UserName$`となってしまった場合、再度`conda deactivate`と打てば<br>
`UserNamenoMacBook-Pro: UserName$`となって仮想環境から抜けることができます。
<br>
その他condaコマンドで困った場合は、[こちらの記事](https://qiita.com/yakisobamilk/items/867dce8e53824146ce05)を参考にしてみて下さい。

---

### ④仮想環境にNode.jsのインストールをする
`$ conda install -c conda-forge nodejs`

<br>
<br>

## ＜カリキュラムの導入＞
※仮想環境に入ったままの状態で実行してください。

### ⑤作業フォルダの作成 & 移動
※別にいらないと思った方はスキップして⑥に進んでいただいて構いません。<br>
`$ mkdir autumn-lesson && cd autumn-lesson`

### ⑥カリキュラムの取得
`$ git clone https://github.com/Kurogoma939/autumn-front.git`

<br>

## 完了！
導入は完了したので、ここから先はVSCodeなどのIDEを起動して作業してください。
- VSCodeのインストールは[こちら](https://code.visualstudio.com/)<br>
- VSCodeのエンジニア向けのおすすめプラグインは[こちら](https://qiita.com/ucan-lab/items/e85931bf8276da43cc97)を参考にしてください。
- Node.js向けの便利なプラグインは[こちら](https://crieit.net/posts/VSCode-Web)を参考にしてください。

<br>
<br>

### ＜中級課題の環境構築＞
中級課題の環境構築で使うと思うので、手順だけこちらにも掲載しておきます。<br>
必要な段階でやって下さい。本体カリキュラムは[こちら](https://mm0311.backlog.jp/wiki/AUTUMN_EDUCATION/%E3%82%AB%E3%83%AA%E3%82%AD%E3%83%A5%E3%83%A9%E3%83%A0%EF%BC%88%E4%B8%AD%E7%B4%9A%EF%BC%89%2F%E7%92%B0%E5%A2%83%E6%A7%8B%E7%AF%89%2F00_%E7%92%B0%E5%A2%83%E6%A7%8B%E7%AF%89)
<br>
#### 00_環境構築
こちらはNode.jsを入れるだけで、上記の環境構築の段階でできているので特に作業はありません。
動作確認として、仮想環境にある状態で`$ node -v` と打ってバージョンが表記されれば問題ありません。

#### 01_webpack

###### 作業フォルダまで移動
`$ cd work/01-webpack`

###### 初期化・package.jsonの生成
`$ npm init -y`

###### webpackのインストール
`npm install webpack webpack-cli --save-dev`

#### 02_ejs
###### フォルダの移動
`$ cd .. && cd 02_ejs`
###### npm install & 実行
`$ npm install`
`$ npm run start`

###### 次に行くために一旦サーバー停止
サーバーを停止するためには **control + c** で止まります。

動作確認  [localhost:9000](http://localhost:9000)

#### 03_sass
###### フォルダの移動
`$ cd .. && cd 03_sass`
###### npm install & 実行
`$ npm install`
`$ npm run start`
