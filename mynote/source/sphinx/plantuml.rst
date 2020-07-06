================
 PlantUMLを使う
================


PlantUMLの配置
==============

ダウンロード
------------

PlantUMLは, 下記ページからダウンロードします.
また, 動作させるためにJavaが必要になります.

- PlantUML
  
  https://plantuml.com/ja/download

  .. figure:: images/plantuml/plantuml-download.png
  

- Java

  https://www.oracle.com/java/technologies/javase-downloads.html
  

配置
----

1. Javaをインストールし, システム環境変数Pathを編集し, ``java`` コマンドが使えるようにしておきます.
2. 上記でダウンロードしたファイルを任意のフォルダに配置します.
   本ドキュメントでは, ``C:\PlantUML`` というフォルダに配置するとします.

sphinxcontrib-plantumlのインストール
------------------------------------

コマンドプロンプトを開き, 下記のコマンドを実行します.

::

   C:\>easy_install sphinxcontrib-plantuml

   
conf.py
=======

