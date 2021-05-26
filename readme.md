# IntelliJ 便利技

- ctrl + o, [は使っておきたい
- double shift
- alt + ctrl + o
- shift + ctrl + o
- shift + ctrl + A
- git annotation

- https://resources.jetbrains.com/storage/products/intellij-idea/docs/IntelliJIDEA_ReferenceCard.pdf

## 検索

### クラスを探してジャンプ

- ctrl + O
- ctrl + O ct

- TLE や time\*exec で、TimeLimitedExecutor を探せる

- ctrl + [・・・ジャンプ前に戻る (windows:ctrl + ←)

### メソッド探してジャンプ

- alt + ctrl + O (windows は shift + ctrl + alt + n)

- 例：TimeLimitedExecutor.getName() を探す => alt + ctrl + o で、getName とするか、TLE.getName でもいける

- alt + ctrl + [・・・ジャンプ前に戻る (windows:alt + ctrl + ←)

### プロジェクト探してジャンプ

- shift + ctrl + O (windows: shift + ctrl + N)
- slash をつけるとフォルダ名と区別しやすい　（resource/file など resource/でも

### 設定(アクション)を探してジャンプ

- ctrl + shift + A
- 例：java compiler、などで探すと設定画面の該当箇所へ

### タブ移動、履歴移動

- shift + ctrl + A・・・タブ検索
- ctrl + E・・・最近開いたファイル
- shift + ctrl + E・・・最近編集したファイル

### グローバルサーチ

- double shift （shift + shift
- tab で section 移動

## short cut

- shift + alt + ↑↓ ・・・ move line up/down
- shift + ctrl + ↑↓・・・ move statement up/down

### 探し方

- keymap で検索できる

### テキストナビゲーション

- 文字ごと：alt 押しながら(mac)
- 端に移動：ctrl + ←→ (mac)

- fn + ctrl + ← ・・・java ソースの最初へ(mac)
- fn + ctrl + → ・・・java ソースの終端へ(mac)
- fn + ↑↓・・・java ソースのページ単位移動

- shift + alt + down ・・・指定行を移動できる（cut paste のかわり)
- shift + ctrl + updown・・・メソッド単位（for ループのブロック単位でも可能)に移動。(cut and paste のかわり)

### コピー・削除

- ctrl + D・・・コピー
- ctrl + delete・・・削除 (windows は ctrl + Y)

### 引数情報表示

- ctrl + P xxxx()のかっこの中にカーソル合わせて ctrl + P

### コメント

- ctrl + /
- shift + ctrl + / ・・・uncomment

### method 折り畳み

- ctrl + マイナス
- ctrl + プラス、でもどる

## 編集

### 選択

- shift + alt + → ・・・範囲選択をジャンプで
- shift + ctrl + → ・・・行選択

- alt + ↑ ・・・文字列全体を設定 => 上を押すたびに選択範囲が広がる (windows・・・ctrl + W , shift + ctrl + W)

### 候補表示

- shift + ctrl + space で候補表示 (new class 名など)
- shift + ctrl + space を 2 回でも出る(候補が広いとき)

```
Calendar calendar = new ;のとき
```

- space2 回・・・メソッドからクラス＋メソッド
- alt + Enter ・・・static import

```
assertSameでspace2回
=> Assert.assertSame()を候補表示
```

### テンプレート表示・変換

- shift + ctrl + A => postfix completion でテンプレート一覧表示できる。下記は一例
- command + J で postfix completion suggestion list 表示

```

s.notnull
=> 変換
if (s != null) {}


s.try
=>
try {
  s
} catch (Exception e) {

}

s.for
→
for (String item: s) {

}


s.fori
→
for (int index=0;////)

forr => iterator
```

### code generator

- command + n => constructor, getter/setter

### コードフォーマット

- google style を導入する。別途しらべる。コマンドでのフォーマットより効率的

### import 整理

- ctrl + alt + O
- 設定：auto import : java optimize imports on the fly => on

### language injection

- alt + enter
- command + W (windows ctrl + F4)
  ※json を injection できるとか？

## git

※git 用コマンドは別途調べる <br>

- ctrl + V・・・git 関連 menu => 対応する数字を押しとメニュークリックされる

- command + D ・・・show diff in commit change
- alt + command + Z ・・・revert file in commit change

- ctrl + v => 7 => branch 表示

- git annotation・・・該当行がどのコミットでできたのかの情報を表示　＝＞　該当の commit-id をクリックすると、そのコミットの変更対象などがわかる

## settings

- Keymap
