---
title: Computing Environment Setup
---
## Computing Environment Setup / 計算環境構築

Set up a standard operating and development environment in Takahashi Lab.
/ 高橋研究室標準の実行・開発環境を構築する。

<i class="fas fa-hammer"></i> 
<i class="fas fa-hammer"></i> 
<i class="fas fa-hammer"></i> 
**The following is under construction. / 以下は作成途中です。**
<i class="fas fa-wrench"></i> 
<i class="fas fa-wrench"></i> 
<i class="fas fa-wrench"></i> 

---

**A. 前提**

[MacOS Big Sur](https://www.apple.com/jp/macos/big-sur/) (MacOS Ver. 11)
（[ユーザーガイド](https://support.apple.com/ja-jp/guide/mac-help/welcome/mac)）

**B. システム環境設定...**

0. Dockとメニューバー > 「Dockを自動的に表示/非表示」をチェック
0. ユーザーとグループ > 変更するにはカギをクリックします。 > ログインオプション > 「”スリープ”、”再起動”、”システム終了’ボタンを表示」をアンチェック
0. ソフトウェア・アップデート > 詳細... > 「macOSアップデートをインストール」以外をチェック
0. Bluetooth > 「メニューバーにBluetoothを表示」をチェック
0. キーボード > 修飾キー... > 「Caps Lockキー」に「Control」、「Controlキー」に「Caps Lock」を割り当てる
0. ショートカット > 入力ソース > 「^スペース」をクリックし、コマンドキーとスペースキーを入力 > Spotlight > 「⌘スペース」をクリックし、コントロールキーとスペースキーを入力
0. 共有 > コンピュータ名を入力 > 「画面共有」、「ファイル共有」、「リモートログイン」をチェック
0. デスクトップとスクリーンセーバー > ホットコーナー... > 右上に「画面をロック」をチェック

**C. Dockの順序**

0. ターミナル　※追加
0. アクティビティ モニタ　※追加
0. Xcode　※追加

**D. 各アプリのインストールと設定**

0. Xcode
- アップルメニュー > App Store... > 開発する > Xcode > 入手 > 開く

0. ターミナル<br>
- アップルメニュー > 環境設定... > 一般 > 「起動時に開く：」は「Homebrew」
- アップルメニュー > 環境設定... > プロファイル > Homebrew > シェル > 「シェルの終了時：」は「シェルが正常に終了した場合は閉じる」> デフォルト
- アップルメニュー > 環境設定... > プロファイル > テキスト > フォントの「変更...」 > Andale Mono 18（好み）
- アップルメニュー > 環境設定... > プロファイル > ウインドウ > ウインドウサイズを列: 110、行: 55（好み）

0. Homebrew
- Homebrewの[サイト](https://brew.sh/index_ja)を開く > 「インストール」の下のスクリプトをコピー > ターミナルを起動 > ペーストして実行

0. Evernote
- アップルメニュー > App Store... > Evernoteを検索  > 入手 > 開く
- 表示オプション > サイドリスト、列は更新日のみにチェック

0. Dropbox
- Dropboxの[サイト](https://www.dropbox.com/desktop)からデスクトップアプリのインストーラをダウンロードしてインストール

0. LINE
- アップルメニュー > App Store... > LINEを検索  > 入手 > 開く

**D. Homebrewの使用法**

※以下の作業はすべてターミナルで行う。

0. 高頻度コマンド
- brew update　Homebrewの更新（formula情報も更新される）
※formulaとはHomebrewが管理しているパッケージの情報
- brew upgrade　Homebrewとインストール済みパッケージの更新、formula名を指定すると当該パッケージのみ更新
- brew install formula名　formulaのインストール
- brew list　インストール済みパッケージのリスト
- brew uninstall formula名　formulaのアンインストール
- brew info formula名　formula情報


0. 低頻度コマンド
- brew cask install アプリ名
- brew outdated　更新されているインストール済みformulaの確認
- brew cleanup　古いバージョンのformulaの削除、-nを付けると削除しないでリストのみ、通常は30日で自動で削除される

