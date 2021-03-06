.. _category-images-of-text:

画像化されたテキスト
----------------------------------------

これらのガイドラインは、テキストを画像化して利用する場合を対象としています。

たとえば写真に写っている人物の名札にある名前、図中のテキスト・ラベルなど、文字情報以外の視覚的情報が、コンテンツのより重要な要素となっているようなものは、このガイドラインの対象外です。

注： WCAG 2.1では ``images of text`` という用語が用いられ、WCAG 2.1日本語訳では「文字画像」という訳語が当てられています。

参考： :ref:`exp-iot-usage`

.. _iot-avoid-usage:

使用の回避
~~~~~~~~~~

.. _gl-iot-avoid-usage:

[MUST] 原則として画像化したテキストを使用しない
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 画像化されたテキストを用いないと実現できない表現が不可欠な場合（例： ロゴ）を除いて、文字情報は画像化せず、テキスト・データで提供する。画像化されたテキストを用いる場合は、以下に示すコントラスト比に関する要件と、代替情報に関する要件を満たす。
チェック内容
   *  |visual|、|markup|： 画像化されたテキストは、自社および他社のロゴ、バナー以外には用いられていない。

.. raw:: html

   <div><details>

意図
````

スクリーン・リーダーのユーザーかアクセスしやすい形で情報を提示する。

テキスト情報の扱いやすさを損ねない。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.4.5:

   *  |SC 1.4.5|
   *  |SC 1.4.5ja|

.. raw:: html

   </div></details>

.. _iot-usage:

画像化されたテキストを使用する場合
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _gl-iot-provide-text:

[MUST] テキスト情報の提供
^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 画像に含まれる文字情報をテキストでも提供する。
チェック内容
   *  |markup|： 画像化されているテキストと同じ内容がスクリーン・リーダーなとで確認できる。

.. raw:: html

   <div><details>

意図
````

スクリーン・リーダーのユーザーが画像化されたテキストにアクセスできるようにする。

参考
````

*  :ref:`exp-iot-text-alternative`

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.1.1:

   *  |SC 1.1.1|
   *  |SC 1.1.1ja|

.. raw:: html

   </div></details>

.. _gl-iot-adjacent-contrast:

[MUST] 隣接領域とのコントラスト比の確保
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 隣接領域の色とのコントラスト比を3:1以上にする。
チェック内容
   *  |visual|： 画像化されたテキストの隣接領域の色とのコントラストが3:1以上になっている。

.. raw:: html

   <div><details>

意図
````

ロービジョン者が、コンテンツを利用できるようにする。

参考
````

*  :ref:`exp-contrast`
*  :ref:`exp-check-contrast`

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.4.11:

   *  |SC 1.4.11|
   *  |SC 1.4.11ja|

.. raw:: html

   </div></details>

.. _gl-iot-text-contrast:

[MUST] 画像内のテキストのコントラスト比
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 画像内のテキストの色と背景の色に十分なコントラスト比を確保する。

   -  テキストの文字サイズが30px（22pt）以上の場合： 3:1以上（[SHOULD] 4.5:1以上）
   -  テキストの文字サイズが22px（18pt）以上で太字の場合： 3:1以上（[SHOULD] 4.5:1以上）
   -  その他の場合： 4.5:1以上（[SHOULD] 7:1以上）

チェック内容
   *  |visual|： 画像化されたテキストにおいて、画像内のテキストの色と背景の色に十分なコントラストが確保されている。

.. raw:: html

   <div><details>

意図
````

ロービジョン者が、コンテンツを利用できるようにする。

参考
````

*  :ref:`exp-contrast`
*  :ref:`exp-check-contrast`

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.4.3:

   *  |SC 1.4.3|
   *  |SC 1.4.3ja|

*  SC 1.4.6:

   *  |SC 1.4.6|
   *  |SC 1.4.6ja|

.. raw:: html

   </div></details>
