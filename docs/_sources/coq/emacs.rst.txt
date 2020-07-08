================
EmacsでCoqを使う
================

環境変数の設定
==============

coqtopコマンドのあるディレクトリに,
パスを通します.
Windowsの場合は, システム環境変数Pathに,
``C:\Coq\bin`` を追加すします.

proof-generalパッケージのインストール
=====================================

elpaからproof-generalパッケージをインストールします.

.. code-block:: elisp

   (package-install 'proof-general)

使い方
======

特に何も設定しなくても, 拡張子 ``.v`` のファイルを開くと,
coq-modeになります.
主なキーバインドは以下の通りです.

.. list-table:: coq-modeのキーバインド

   * - C-c C-n
     - 1ステップ進む
   * - C-c C-u
     - 1ステップ戻る
   * - C-c C-Enter
     - カーソル位置まで進める

その他のキーバインドは, 以下参照.

- http://proofcafe.org/wiki/ProofGeneral

- http://proofcafe.org/wiki/ProofGeneral/Keybinds
