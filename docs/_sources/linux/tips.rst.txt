============
 Linux Tips
============

ユーザをsudoに追加する
======================

rootユーザで, adduserコマンドでsudoグループに追加します.

.. code-block::

   # adduser <ユーザ名> sudo

システムを再起動すると反映されます.
以下のコマンドで確認します.

.. code-block::

   $ sudo -v
