---
title: "Siv3D プログラミング上達ガイドライン"
free: true
---

# Siv3D プログラミング上達ガイドライン
Siv3D の機能をフル活用し、生産的で間違いが少ない、実行時性能に優れたプログラムを書くためのガイドラインです。

## 1. 一般的なコーディング

#### 標準ライブラリよりも Siv3D の機能を優先しよう


#### 不必要な C++ 標準ライブラリはインクルードしないようにしよう


#### Siv3D の提供する数学定数を使おう


#### コンパイラの警告に敏感になろう


#### フレームレートに依存する処理を作らないようにしよう


#### 読み込みたいファイルを配置するディレクトリを理解しよう




## 2. アセットを扱う

#### アセットはポインタで管理する必要が無いことを理解しよう

#### アセットをグローバル変数で扱わないようにしよう

#### アセットを static 変数で扱わないようにしよう

#### 縮小表示する画像ファイルは `TextureDesc::Mipped` を指定しよう


## 3. 実行時性能

#### 配列や文字列、アセットを関数に渡すときは const 参照渡しを使おう

#### メインループ内で重いオブジェクトを作成しないようにしよう

#### Siv3D の関数の呼び出し回数を抑えよう

#### グリッド上に並ぶ大量の点や正方形を描く場合、`Image` の使用を検討しよう

#### 内部の Draw コールの回数を抑えよう


## 4. 開発生産性

#### 再ビルドしなくても良い開発手法を知ろう



