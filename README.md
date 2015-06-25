# CSSのクラス名に使える単語
OOCSS、SMACSS、BEM、FLOCSSなどCSS設計のためのガイドラインはいくつも出ていますが、実際にコーディングする時に迷ってしまうのがどのようなクラス名を使用するのかということ。

CSS設計において正解はありません。どのガイドラインを参考にしてもいいですが**一度決めたルールを守り続けること**を破ってしまうと、どんなに優れたガイドラインを定めても意味がありません。

`.wrapper`なのか`.container`なのか、`.button`なのか`.btn`なのか。同じ意味でも単語が違ったり、省略するのかそうでないのかなど制作会社や個人個人によって違いが出ます。

ここでは推奨する単語を定めてはいません。色々な単語を集めて分類することで比較し、ルールを明確に定義するためのツールとして作成をしています。

## アウトライン
HTML5におけるsection, article, nav要素のようにアウトラインを形成するセクションとそれに付随する要素。

### セクション
* section
* article, main, entry, entries, content, contents, site
* aside, side, sidebar, secondary, second
* header, head
* footer, foot
* navigation, nav, menu
* home, top

### セクションに関連する要素
* heading, headline, title
* logo
* description(概要、説明、解説)
* hero, visual, jumbotron, cover（ファーストビューに配置する大きめの画像）
* copyright, small
* form

## レイアウト
CSSでレイアウトを指定する際に使用する。

### ブロック
* wrapper, container, outer, area（要素のかたまりを物理的にまとめるために使用される）
* inner, body, box, unit, holder, frame（wrapperやcontainerなどに入れ子にして配置するコンテナブロック）
* list, items（ul要素やol要素のような箇条書きや一覧）
* group, collection（同じ分類の要素をまとめる）
* grid（グリッドレイアウトを使用する時にルートになる）
* row（グリッドレイアウトを使用する時のclearfixや行を指定する）
* column, columns, col（グリッドレイアウトを使用する時の列の横幅を指定する）
* media（画像と文章が横並びになったもの）
* card（画像と文章が縦並びになったもの）
* tile, panel（複数の同じ形状のブロックを並べたもの）

### エレメント
* item, cell（ブロックに内包される汎用的な名前）
* link
* text, message, sentence（文章）
* caption（図表を補足する）
* summary（概要、要約）
* note（注釈、注意）
* lead（見出しの補足や記事の要約）

### モディファイア
エレメントやコンポーネントのバージョン違い。恒久的で状態が変化しない。

* push
* pull
* fluid（内包されている要素によってサイズが可変する）
* fixed, sticky（fixedは固定、stickyは指定された位置から固定）
* reverse（反転する）
* left
* right
* center
* huge, large
* medium, normal
* small, tiny
* author
* guest, user
* previous, next

### ステート
モディファイアと違いユーザーの操作などで状態が変化する。

* active, current（複数の選択肢のうち現在選択されている状態）
* disabled（機能が無効になっている状態）
* visible, show（見せる、表示する）
* invisible, hide, hidden（隠す、非表示にする）
* open, opened（開く）
* close, closed（閉じる）
* alert, error, warning, danger（警告、エラー）
* success
* information, info 

## プレフィックス
クラス名の重複を避けたり意図を明確にするため、ブロックやコンポーネントにプレフィックス（接頭辞）を付与する。

* site, common（共通の）
* global, main（主要な）
* top（トップページの）
* local
* brand（サイトを象徴するカラーやフォント）
* is-（ある状態になった）
* has-（ある状態になっている）
* l-, layout（ヘッダーやコンテンツ部分などのコンテナブロック）
* p-（汎用的でないプロジェクト固有のパターン）
* c-（汎用性があり再利用できるパターン）
* u-（`mb-10`や`clearfix`といった単一の目的に使用するクラス）

## コンポーネント
ボタンやタブといった汎用的に使用される要素。

* grid
* button, btn
* tab, tabs
* toggle（同じ操作で状態を切り替えられる）
* dropdown（複数の値から選択できるリスト）
* modal, daialog（確認や警告のため、基本的に自動で表示され、消すまでは元の画面に戻れない）
* lightbox
* carousel, slider（コンテンツを水平・垂直にスライド表示させる）
* accordion（タイトルとそれに対応したコンテンツを表示させる）
* off-canvas（画面がスライドしてナビゲーションを表示させる）
* tooltip, popover
* breadcrumb（パンくずリスト）
* search
* pagenation, pager
* progress, progressbar
* label
* badge
* caret
* arrow


## 画像

* image, img, photo
* thumbnail（画像を一覧表示するために縮小して表示させたもの）
* avatar（ユーザーやゲストを識別するための画像）
* feature（対応する文章の特徴を補足するための画像やイラスト）
* overlay（要素の上の階層に覆いかぶさる）
* AdSense, ad, banner, pr（Googleのアドセンスや広告）
* icon


## コンテンツ
コンテンツ部分で使用する。

* about
* staff, member
* menu, shop, online
* work, works, product
* news, event, topic, pickup
* history
* concept
* comment
* contact, inquiry（お問い合わせ）
* access
* date
* category
* tag
