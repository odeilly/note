========
 テーマ
========

Sphinxでは, 10個の組み込みテーマがあります.
また, サードパーティ製のテーマを利用することもできます.

サードパーティ製のテーマの1つである,
bootstrapのテーマをインストールします.

https://github.com/ryan-roemer/sphinx-bootstrap-theme


テーマのインストール
====================

コマンドプロンプトで, 下記を実行します.

::

   C:\>pip install sphinx_bootstrap_theme

bootstrapテーマを適用する
=========================

conf.py に, 以下を追加します.

::

   # At the top.
   import sphinx_bootstrap_theme

   #...

   # Activate the theme.
   html_theme = 'bootstrap'
   html_theme_path = sphinx_bootstrap_theme.get_html_theme_path()
   
