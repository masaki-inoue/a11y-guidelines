.. _category-link:

リンク
--------------------------

これらのガイドラインは、リンクに関するものです。

ここでリンクとは、ユーザーがクリック（タッチ）することでページ遷移や何らかの機能が実行されるものを差します。
リンクにはテキストのみで構成されているもの、アイコンが用いられているもの、画像とテキストの一方又は両方が用いられているものが含まれます。
また、 ``a`` 要素で実装されているものに加えて、 ``button`` 要素で実装されていたり、適切な ``role`` 属性が付加されて実装されているものも含みます。

.. _link-perceivable:

認知を可能にする
~~~~~~~~~~~~~~~~

.. _gl-link-color-only:

[MUST] 複数の視覚的要素を用いた表現
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] クリッカブルであることを、色だけで表現しない。
チェック内容
   *  |visual|： グレースケール表示にしたとき、どの部分がリンクか判別できる。（例： リンクに下線があるなど）

.. raw:: html

   <div><details>

意図
````

視覚障害者や色弱者がリンクを認知できるようにする。

参考
````

*  :ref:`exp-color-only`
*  :ref:`exp-grayscale`

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.4.1:

   *  |SC 1.4.1|
   *  |SC 1.4.1ja|

.. raw:: html

   </div></details>

.. _gl-link-text:

[MUST] 適切なリンク・テキスト
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] リンク・テキスト（``a`` 要素の中身、アイコンのラベルなど）は、そのリンクの目的を判断できるものにする。
チェック内容
   *  |visual|： 「○○はこちら」の「こちら」の部分だけがリンクになっていない。（この場合は「○○はこちら」全体をリンクにする。）、または
   *  |visual|： リンク・テキストの意図がマークアップで明確になっている。（事例参照）

.. raw:: html

   <div><details>

意図
````

リンク先を閲覧するかどうかの判断を容易にして、肢体不自由者の不必要な操作の抑制につなげる。

スクリーン・リーダーが提供するリンクの一覧機能を使う視覚障害者が、リンク先について容易に判断できるようにする。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 2.4.4:

   *  |SC 2.4.4|
   *  |SC 2.4.4ja|

例
``

.. list-table:: 注意すべきリンク・テキストの文言（「」部分がリンク・テキスト）
   :header-rows: 1

   *  -  NG
      -  OK
   *  -  ○○は「こちら」
      -  「○○はこちら」
   *  -  「もっと見る」
      -  「○○についてもっと見る」
   *  -  「詳細」
      -  「○○についての詳細」

.. todo:: マークアップで意図が明示できている例を追加

.. raw:: html

   </div></details>

.. _gl-link-consistent-text:

[MUST] 一貫したリンク・テキスト
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 同じ機能を実行するリンクは、サイト内で一貫性のあるリンク・テキストを付与する。
チェック内容
   *  |visual|： 同じ目的で設置されているリンクには、サイト内で一貫したリンク・テキストが用いられている。

.. raw:: html

   <div><details>

意図
````

予測可能性を上げ、混乱を防ぐ。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 3.2.4:

   *  |SC 3.2.4|
   *  |SC 3.2.4ja|

.. raw:: html

   </div></details>

.. _gl-link-tab-order:

[MUST] 適切なフォーカス順序
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] Tab/Shift+Tabキーでフォーカスを移動させたとき、コンテンツの意味に合った適切な順序でフォーカスを移動させる。
チェック内容
   *  |behavior|： Tab/Shift+Tabキーを使ってリンク間でフォーカスを移動させたとき、レイアウト的にも文脈的にも自然な順序でフォーカスが移動する。

.. raw:: html

   <div><details>

意図
````

スクリーン・リーダーなどの支援技術がコンテンツを正しく認識し、ユーザーに適切な形で提示できるようにする。

参考
````

*  :ref:`exp-tab-order-check`

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 2.4.3:

   *  |SC 2.4.3|
   *  |SC 2.4.3ja|

.. raw:: html

   </div></details>

