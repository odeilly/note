========
 テーマ
========

Sphinxでは, 10個の組み込みテーマがあります.
また, サードパーティ製のテーマを利用することもできます.

Sphinx Theme for Basicstrap を利用する
======================================

https://pythonhosted.org/sphinxjp.themes.basicstrap/index.html

ダウンロード
------------

コマンドプロンプトで, 下記を実行します.

::

   C:\>pip install sphinxjp.themes.basicstrap

   
適用
----

conf.py に, 以下を追加します.

.. code-block:: python

   extensions = [

       ...

       'sphinxjp.themes.basicstrap',

       ...
       
   ]

   html_theme = 'basicstrap'


Sphinx Bootstrap Themeを利用する
================================

https://github.com/ryan-roemer/sphinx-bootstrap-theme

ダウンロード
------------

コマンドプロンプトで, 下記を実行します.

.. code-block:: none

   C:\>pip install sphinx_bootstrap_theme

適用
----

conf.py に, 以下を追加します.

.. code-block:: python

   # At the top.
   import sphinx_bootstrap_theme

   #...

   # Activate the theme.
   html_theme = 'bootstrap'
   html_theme_path = sphinx_bootstrap_theme.get_html_theme_path()
   
Read the Docs テーマを利用する
==============================

https://sphinx-rtd-theme.readthedocs.io/en/stable/

ダウンロード
------------

コマンドプロンプトで, 下記を実行します.

::

   pip install sphinx-rtd-theme
   

適用
----

conf.py に, 以下を追加します.

.. code-block:: python

   import sphinx_rtd_theme

   extensions = [

       ...

       'sphinx_rtd_theme',

       ...

   ]

   html_theme = 'sphinx_rtd_theme'

   
Bootstrap v4 HTML Theme for Sphinx を利用する
=============================================

https://github.com/myyasuda/sphinxbootstrap4theme

ダウンロード
------------

コマンドプロンプトで, 下記を実行します.

::

   pip install sphinxbootstrap4theme

適用
----

.. code-block:: python

   import sphinxbootstrap4theme

   html_theme = 'sphinxbootstrap4theme'
   html_theme_path = [sphinxbootstrap4theme.get_path()]
   
