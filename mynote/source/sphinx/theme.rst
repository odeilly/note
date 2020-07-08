========
 テーマ
========

Sphinxでは, 10個の組み込みテーマがあります.
また, サードパーティ製のテーマを利用することもできます.

.. Sphinx Foundation Theme を利用する
   ==================================
    
   https://github.com/peterhudec/foundation-sphinx-theme
    
    
   インストール
   ------------
    
   コマンドプロンプトで, 下記を実行します.
    
   ::
    
      pip install foundation-sphinx-theme
    
    
   適用
   ----
    
   conf.py に, 以下を追加します.
    
   .. code-block:: python
    
      import foundation_sphinx_theme
    
      extensions = [
    
          ...
    
          'sphinx.ext.autodoc',
          'foundation_sphinx_theme',
    
          ...
          
      ]
    
      html_theme = 'foundation_sphinx_theme'
    
      


Sphinx Theme for Basicstrap を利用する
======================================

https://pythonhosted.org/sphinxjp.themes.basicstrap/index.html

インストール
------------

コマンドプロンプトで, 下記を実行します.

::

   pip install sphinxjp.themes.basicstrap

   
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

オプション
----------

テーマオプションは, 下記ページを参照して下さい.

https://pythonhosted.org/sphinxjp.themes.basicstrap/options.html#sample-and-html-theme-options


Sphinx Bootstrap Themeを利用する
================================

https://github.com/ryan-roemer/sphinx-bootstrap-theme

インストール
------------

コマンドプロンプトで, 下記を実行します.

.. code-block:: none

   pip install sphinx_bootstrap_theme

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

インストール
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

インストール
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
   
