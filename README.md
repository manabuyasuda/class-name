# CSSのクラス名に使われる単語一覧
OOCSS、SMACSS、BEM、FLOCSSなどCSS設計のためのガイドラインはいくつも出ていますが、実際にコーディングする時に迷ってしまうのがどのようなクラス名を使用するのかということ。

同じような意味の`.wrapper`と`.container`のどちらを使うのか、`.button`と`.btn`のように省略は許容するのか。コードを書く人によってばらつきが出たり、感覚的に書いていると区別もなく両方使ってしまったりします。

ここでは推奨する単語を定めてはいません。色々な単語を集めて分類・比較し、ルールを明確に定義するためのツールとして作成をしています。

## アウトライン
HTML5におけるsection, article, nav要素のようにアウトラインを形成するセクションとそれに付随する要素です。

### セクション
単一の単語ではなく`.l-header`や`.mainNavigation`のようにプレフィックスを付与することで一意で明確な意図を示すこともできます。

* section
* article, main, entry, entries, content, contents, site
* aside, side, sidebar, secondary, second
* header, head
* footer, foot
* navigation, nav, menu
* home, top
* single（個別記事、シングルページ）
* post

### セクションに関連する要素
* heading, headline, title
* lead（見出しの補足や記事の要約）
* logo（サイトロゴ）
* copyright, small（コピーライト）
* widget
* popular, ranking（人気記事、ランキング）
* privacy（プライバシーポリシー）
* sitemap（サイトマップ）


## レイアウト
CSSでレイアウトを指定する際に使用します。BEMとSMACSSの分類方法を使用しています。セクションと同じくプレフィックスを付与してバリエーションを作ります。

### ブロック
* wrapper, wrap, container, outer, area（要素のかたまりを物理的にまとめるために使用される大枠のコンテナブロック）
* inner, body, box, unit, holder, frame, region（wrapperやcontainerなどに入れ子にして配置するコンテナブロック）
* list, items（ul要素やol要素のような箇条書きや一覧）
* group, collection（同じ分類の要素をまとめる）
* grid（グリッドレイアウトを使用する時にルートになる）
* row（グリッドレイアウトを使用する時のclearfixや行を指定する）
* column, columns, col（グリッドレイアウトを使用する時の列の横幅を指定する）
* media（画像と文章が横並びになったもの）
* card（画像と文章が縦並びになったもの）
* tile, panel（複数の同じ形状のブロックを並べたもの）
* form
* video, player（動画）
* mask, overlay, blur（要素の上の階層に覆いかぶさって見た目を変化させる）


### エレメント
* item, cell（ブロックに内包される汎用的な名前）
* link
* tagline, slogan（スローガン、キャッチコピー）
* catch, copy（キャッチコピー）
* text, message, sentence（文章）
* caption（図表を補足する）
* summary（概要、要約）
* note（注釈、注意）
* description, desc（概要、説明、解説）
* introduction（紹介する、前置き、解説）
* announce（告知、お知らせ）
* information, info 
* meta（メタ情報）
* target
* previous, next

### モディファイア
エレメントやコンポーネントのバージョン違い。恒久的で状態が変化しません。汎用クラスにも使用できます。

* push
* pull
* fluid（内包されている要素によってサイズが可変する）
* fixed, sticky（fixedは固定、stickyは指定された位置から固定）
* reverse（反転する）
* left
* right
* center
* top
* middle
* bottom
* huge, large
* medium, normal
* small, tiny
* author
* guest, user
* sp, mobile, tb, pc（スマホ、タブレット、パソコン）

### ステート
モディファイアと違いユーザーの操作などで状態が変化する。

* active, current（複数の選択肢のうち現在選択されている状態）
* disabled（機能が無効になっている状態）
* visible, show（見せる、表示する）
* invisible, hide, hidden（隠す、非表示にする）
* open, opened（開く）
* close, closed（閉じる）
* alert, error, caution, warning, danger（警告、エラー）
* success（成功）


## プレフィックス
クラス名の重複を避けたり意図を明確にするため、ブロックやコンポーネントにプレフィックス（接頭辞）を付与する。

* site, common（共通の）
* global, main（主要な）
* sub（補助的な）
* general（一般的な、全体的な）
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
* modal, daialog（確認や警告のため表示される）
* lightbox
* carousel, slider（コンテンツを水平・垂直にスライド表示させる）
* accordion（タイトルとそれに対応したコンテンツを表示させる）
* off-canvas（画面がスライドしてナビゲーションを表示させる）
* tooltip, popover
* breadcrumb（パンくずリスト）
* search
* pagenation, pager
* backtop（トップへ戻る）
* progress, progressbar
* label
* badge
* caret
* arrow


## 画像
主に画像の形式で使用される要素。

* image, img, photo
* hero, visual, jumbotron, cover（ファーストビューに配置する大きめの画像）
* thumbnail（画像を一覧表示するために縮小して表示させたもの）
* avatar（ユーザーやゲストを識別するための画像）
* feature（対応する文章の特徴を補足するための画像やイラスト）
* gallery
* AdSense, ad, sponsor, advertise, banner, pr（Google Adsenseや広告）
* icon


## コンテンツ
コンテンツ部分で使用する要素。

* about
* staff, member
* menu, shop, online
* work, works, product
* news, event, topic, pickup
* history, archive
* concept
* recommend
* toc, index（目次）
* comment
* contact, inquiry（お問い合わせ）
* access
* map
* sns, social, share（ソーシャルボタン）
* date, time, published
* category, categories, cat
* tag
* address
* tel, phone
