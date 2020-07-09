======
 メモ
======

シンタックスハイライト
======================

https://www.sphinx-doc.org/ja/master/usage/restructuredtext/directives.html#code-examples

ハイライトできる言語は, Pygmentsがサポートしている全ての言語です.
以下のページに掲載されています.

https://pygments.org/docs/lexers/

シンタックスハイライトの例
--------------------------

.. code-block:: none

   .. code-block:: java

      public class Sample {
          public static void main(String[] args) {
              System.out.println("Hello.");
          }
      }


.. code-block:: java

   public class Sample {
       public static void main(String[] args) {
           System.out.println("Hello.");
       }
   }


ソースコードのインポート
------------------------

``.. literalinclude:: filename`` を使うと,
外部のソースコードをインポートすることができます.

.. code-block:: none

   .. literalinclude:: Sample.java
      :language: java


.. literalinclude:: Sample.java
   :language: java
