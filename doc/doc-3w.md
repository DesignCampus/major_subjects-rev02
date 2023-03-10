---
theme: "simple"
customTheme : "my-theme"
transition: "convex"
slideNumber: false
title: "コーディング 2nd Season 3w - JavaScript"
---

# コーディング<br>ライブ授業
<h2 class="firstPage"><small>後期3週目</small><br>「JavaScript」</h2>
<img src="./img/logo_bg_none.png" style="width: 16%;">

---

1. 受講生MTG
1. はじめに
1. 座学
1. 実習
1. 講師FB
1. まとめ
1. 受講生MTG

---

## 受講生MTG

--

### 卒業制作

--

### クライアントワーク

---

## はじめに

--

### 役割分担

- プロジェクトリーダー
- トップページと共通CSS
- 下層ページ
- JavaScriptと下層ページ等のヘルプ

--

### 先週の課題

--

お気に入りサービスやツールを見つけて、3分で紹介
- 何をするものか
- どこが気に入っているか
- 実際にどうやって活用しているか

--

「おみくじアプリ」
- どんな見た目にするか  
基本要素は結果の表示と実行ボタン
- どんな内容にするか


---

座学の時間
## JavaScript

---

空のHTMLファイルを用意して

---

### 変数スコープ

--

スコープとは参照できる範囲のこと

--

ところで“変数宣言”何があった？

--

宣言 | 内容
-------------|---------------
何もつけない      | グローバル
var      | 関数　再宣言可
let      | ブロック　再宣言不可
const      | ブロック　再宣言不可　定数
[変数宣言の種類]

--

スコープの種類

```txt
├── グローバルスコープ
└── ローカルスコープ
    ├──関数スコープ
    └──ブロックスコープ
```

--

実際に体験してみよう

---


### 配列

--

変数の一種  
複数の値をまとめて管理、格納できる

--

衣装ケースをイメージしてみて

<p><img src="./img/2w/ishou.jpg" style="width: 20%;"><p/>

- Tシャツ
- パンツ
- 靴下

※1つの段にはひとつしかもの（値）が入らないよ

--

#### 配列の書き方

配列名 = [要素1, 要素2, 要素3,　…];

```js
wardrobe = ["Tシャツ", "パンツ", "靴下"]
```

--

#### 参照するには

全部の値：配列名;

```js
wardrobe
```

値を一つだけ：配列名[添え字];

```js
wardrobe[0]
```

※添え字は数字で0から始まります

--

記述 | 内容 | 例
-------------|---------------|---------------
length | 要素の数を調べる | wardrobe.length
push() | 最後に要素を追加 | wardrobe.push("ズボン")
pop() | 最後の要素を削除 | wardrobe.pop()
unshift()| 最初に要素を追加 | wardrobe.unshift("ハンカチ")
shift() | 最初の要素を削除 | wardrobe.shift()
[配列の操作1]

--

記述 | 内容 | 例
-------------|---------------|---------------
slice() | コピーするときなど | 後述
splice() | 任意の位置で追加や削除 | 後述
[配列の操作2]

--


```js
/**
 * slice(コピー開始の位置,コピー終了の位置+1)
 */

//a = wardrobe.slice(1,2);//1番目の要素から1番目の要素までをコピー
a = wardrobe.slice(1,4);//1番目の要素から3番目の要素までをコピー
console.log("sliceの結果：" + a);

```

--

```js
/**
 * splice(削除開始の位置,削除する要素数)
 */

wardrobe.splice(0, 1);// 0番目から1つの要素を消す
console.log("spliceの結果：" + wardrobe);

// 2番目から1つも要素を消さないで、その位置の後ろに要素を追加
letterCase.splice(2, 0, "ズボン");
console.log("spliceの結果2：" + wardrobe);

```

---

### API

--

アプリケーションプログラミングインターフェース

--

- Web API（ウェブAPI）の一覧リスト  
https://it-jog.com/wapi/webapis

- 【2022年最新】これは使える！種類別アプリAPI一覧  
https://engineer-style.jp/articles/1675


--

クジラWeb API
https://api.aoikujira.com/

---

### 何かを作るときのアドバイス


--

作るときには設計を

--

<p><img src="./img/2w/flow.png" style="width: 50%;"><p/>

---

## 実技

--

### ページのトップに戻るボタン
<small>サンプルファイル  
example/js.html</small>

<small>以前の前期  
example/js-0-c.html</small>

<small>以前の後期  
example/js-0-m.html</small>

--

### おみくじの解説
<small>サンプルファイル  
example/omikuji.html</small>

--

### スクロールの監視
<small>サンプルファイル  
example/intersection_observer.html</small>

---

## 実習

--

11:20-11:50まで  
※休憩等は自由に

---

## 来週に向けて

--

おみくじを来週の授業で完成するところまですすめておく

--

### 予告

次週はHTMLとCSSのお話し

座学多めになる予定です



