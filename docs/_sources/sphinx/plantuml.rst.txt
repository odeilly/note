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

1. 上記でダウンロードしたファイル plantuml.jar を任意のフォルダに配置します.
   本ドキュメントでは, ``C:\PlantUML`` というフォルダに配置するとします.
2. Javaをインストールし, システム環境変数Pathを編集し, ``java`` コマンドが使えるようにしておきます.

sphinxcontrib-plantumlのインストール
------------------------------------

コマンドプロンプトを開き, 下記のコマンドを実行します.

.. code-block:: none

   C:\>easy_install sphinxcontrib-plantuml

   
conf.pyの編集
=============

extensions に sphinxcontrib.plantuml を追加します.

.. code-block:: python
   
   extensions = [
   
       ...
       
       'sphinxcontrib.plantuml',
       
       ...
       
   ]

plantuml コマンドを設定します.

.. code-block:: python

   plantuml = 'java -jar /PlantUML/plantuml.jar'

作成例
======

.. code-block:: rst

   .. uml::

      Alice -> Bob: Hi!
      Alice <- Bob: How are you?


.. uml::

   Alice -> Bob: Hi!
   Alice <- Bob: How are you?
