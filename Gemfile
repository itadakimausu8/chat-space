source 'https://rubygems.org'

#デフォルトgem-----------------------------------------------

    # rails導入 バージョンは5.0~5.0.0.1の範囲
    gem 'rails', '~> 5.0.0','>=5.0.0.1'

    # Active Recordで使うデータベースの種類
    gem 'mysql2', '>= 0.3.13', '< 0.5'

    # スタイルシートで使うSCSSの導入
    gem 'sass-rails', '~> 5.0'

    # Uglifierの導入。UglifyJS2より JavaScript のコード軽量化ライブラリを、Ruby で簡単に使えるようできる。要はJavaScriptを圧縮してくれる。
    gem 'uglifier', '>= 1.3.0'

    # coffee-scriptを使えるようにする。coffee-scriptはjavascriptをruby向けに簡単にしたもの。
    gem 'coffee-rails', '~> 4.1.0'

    # JavaScriptのライブラリ「jquery」の導入
    gem 'jquery-rails'


    # Turbolinksを導入する。Turbolinksは画面遷移を高速化させる。主にcssとjavascriptで役に立つ。
    gem 'turbolinks'

    # jubilderの導入。Jsonのテンプレートエンジン
    gem 'jbuilder', '~> 2.0'

    # Rubyのソースコードからコメント等を読み取りHTML+CSS+JavaScriptを吐き出して、ブラウザで閲覧しやすいドキュメントを作ってくれる。
    gem 'sdoc', '~> 0.4.0', group: :doc



#追加したgem--------------------------------------------------------

  #view用
    #railsにてhamlを使えるようにするためのgem
    gem 'haml-rails'



# 開発&テスト用-----------------------------------------------------
  group :development, :test do
    #デバッグ用のgem
    gem 'byebug'
  end



# 開発用-----------------------------------------------------------
  group :development do
    #ビュー内でコンソールを立ててデバッグできるgem
    gem 'web-console', '~> 2.0'

    #hamlに変換できるgem
    gem 'erb2haml'

    #Springと呼ばれるアプリケーションプリローダーを導入する。アプリケーションプリローダーとは事前にバックグラウンドでライブラリをロードしておくことで、その待ち時間を短くするもの。
    gem 'spring'
  end

