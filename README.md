# autumn-front 

### ＜大前提として、エンジニアたる者としてインストールしておきたいもの＞
- brew
## ＜仮想環境の構築手順＞

### ① Anacondaのインストール
[こちらのリンク](https://www.anaconda.com/products/individual#Downloads)から、OSに合うものをインストールしてください。

**ここから先は、「ターミナル（MAC）」または「コマンドプロンプト（Windows）」を起動して行ってください❗️**

### ②condaコマンドを使って仮想環境の構築
ターミナルで以下のコマンドを実行してください。<br>
`$ conda create -n autumn-front`

### ③仮想環境に入る
`$ conda activate autumn-front`

---

#### 〜Anacondaに関する予備知識〜
仮想環境に入れると、ターミナルの表記が
`UserNamenoMacBook-Pro: UserName$`から<br>
`(autumn-front)UserNamenoMacBook-Pro: UserName$`と表記が変わります。<br>
この状態になっていればAnaconda（仮想環境）に入れている証拠です。<br>
<br>
仮想環境から抜けたい場合は、`conda deactivate`と打てば抜けられます。<br>
もしかしたら一度だけでは`(base)UserNamenoMacBook-Pro: UserName$`となり、Anacondaのbase環境に移動してしまう場合があります。<br>
そうなったら再度`conda deactivate`と打てば`UserNamenoMacBook-Pro: UserName$`となって仮想環境から抜けることができます。

---

### ④仮想環境にNode.jsのインストールをする
`$ conda install -c conda-forge nodejs`
<br>

## ＜カリキュラムの導入＞
※仮想環境には入った状態で実行してください。

### ⑤作業フォルダの作成 & 移動
`mkdir autumn-lesson && cd autumn-lesson`

### ⑥カリキュラムの取得
`git clone ~~~~~~ `

<br>

## 完了！
導入は完了したので、ここから先はVSCodeなどのIDEを起動して作業してください。
- VSCodeのインストールは[こちら](https://code.visualstudio.com/)<br>
- エンジニア向けのおすすめプラグインは[こちら](https://qiita.com/ucan-lab/items/e85931bf8276da43cc97)を参考にしてください。
- Node.js向けの便利なプラグインは[こちら](https://crieit.net/posts/VSCode-Web)を参考にしてください。
