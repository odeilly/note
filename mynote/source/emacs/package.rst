===============
 Emacs Package
===============

switch-window
=============

Emacsではウィンドウの切り替えとして C-x o (other-window) があります.
しかし, other-window は,
1つ1つウィンドウ切り替えていきますので,
ウィンドウを多く使っている場合には,
目的のウィンドウに辿り着くまで C-x o を連打する必要があります.

switch-window を導入すれば,
ウィンドウ をキーボードで選択できるようになり,
負担が軽減されます.
しかも, 各ウィンドウのサイズを変更する機能もついてきます.

インストール
------------

Elpa からインストールできます.

.. code-block:: elisp

   (package-install 'switch-window)

設定
----

C-x o を上書きします.
あるいは, C-t に割り当てます.

.. code-block:: elisp

   (global-set-key (kbd "C-t") 'switch-window)

複数のウィンドウを開いて, C-t を実行すると,
各ウィンドウが数字に変換されます.
キーボードで数字を打つと, その数字に対応するウィンドウに切り替わります.

数字はキーボードの上に位置して少々打ちにくいので,
アルファベットで移動できるように変更しましょう.

.. code-block:: elisp

   (setq switch-window-shortcut-style 'qwerty)

今度は, アルファベット (asdf等) で選択できるようになります.

ウィンドウが2個の場合は, わざわざ選択する必要はないので,
アルファベットを出さないように変更します.

.. code-block:: elisp

   (setq switch-window-threshold 2)

アスキーアートや画像を使うこともできます.

.. code-block:: elisp

   (setq switch-window-shortcut-appearance 'asciiart) ;; アスキーアート

.. code-block:: elisp

   (setq switch-window-shortcut-appearance 'image) ;; 画像

ウィンドウを選択する画面で i をタイプすると,
上にあるウィンドウの高さが小さくなり,
下にあるウィンドウの高さが大きくなります.

その他,
以下の表のようになります.

.. list-table::

   * - i
     - 上
   * - k
     - 下
   * - j
     - 左
   * - l
     - 右
   * - b
     - 全てのウィンドウのバランスを整える.
