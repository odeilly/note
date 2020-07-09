===========
 Autobuild
===========

文章の編集を行ない随時確認するために,
autobuildを使用します.

インストール
============

以下のコマンドを実行します.

.. code-block:: none

   pip install sphinx-autobuild

実行
====

以下のコマンドを実行します.

.. code-block:: none

   sphinx-autobuild -b ソースフォルダ  出力先フォルダ

ブラウザで, http://localhost:8000 で開くことができます.
``-p`` オプションでポートを指定することができます.
