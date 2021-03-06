.. _category-multimedia:

音声・映像コンテンツ
------------------------------------------------

これらのガイドラインは、音声のみのコンテンツ、音声を含む動画コンテンツ、映像のみの動画コンテンツに関するものです。

.. _multimedia-perceivable:

存在を認知できる
~~~~~~~~~~~~~~~~

.. _gl-multimedia-perceivable:

[MUST] 音声・映像コンテンツの存在を明示する
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 音声・映像コンテンツの存在を認知できるようにする。
チェック内容
   *  |visual|、|markup|： ページ内に埋め込まれる音声/動画プレイヤーについて、適切なラベル付けがされていてそこにプレイヤーがあることが容易に認知できるようになっている。または
   *  |visual|、|markup|： 前後のテキストから、そこにプレイヤーがあることが推測できる。

.. raw:: html

   <div><details>

意図
````

視覚障害者、聴覚障害者が音声や映像を含むコンテンツの存在を認知できるようにする。

参考
````

*  :ref:`exp-multimedia-perceivable`

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.1.1:

   *  |SC 1.1.1|
   *  |SC 1.1.1ja|

.. raw:: html

   </div></details>

.. _multimedia-operable:

操作や理解を阻害しない
~~~~~~~~~~~~~~~~~~~~~~

.. _gl-multimedia-operable:

[MUST] 音声の自動再生
^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 3秒以上の長さの音声を自動再生しない。
チェック内容
   *  |visual|： 自動再生される音声はない。または
   *  |visual|： 自動再生される音声は3秒以内の長さになっている。

.. raw:: html

   <div><details>

意図
````

スクリーン・リーダーの音声出力を阻害しない。

参考
````

*  :ref:`exp-multimedia-autoplay`

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.4.2:

   *  |SC 1.4.2|
   *  |SC 1.4.2ja|

.. raw:: html

   </div></details>

.. _gl-multimedia-pause-movement:

[MUST] 動きを伴うコンテンツ
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 自動的に開始し5秒以上継続する、アニメーションや動画のなどの視覚的な動きを伴うコンテンツを作らない。
   そのようなコンテンツを作る場合は、ユーザーが一時停止、停止、または非表示にすることができるようにする。
チェック内容
   *  |visual|、|behavior|：自動的に開始し5秒以上続く動画、アニメーションがない。または
   *  動画やアニメーションを呈し、一時停止、または非表示にすることができる。

.. raw:: html

   <div><details>

意図
````

ロービジョン者や認知障害者が、集中を阻害されないようにする。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 2.2.2:

   *  |SC 2.2.2|
   *  |SC 2.2.2ja|

.. raw:: html

   </div></details>

.. _gl-multimedia-no-trap:

[MUST] キーボード・トラップの回避
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] 音声/動画のプレイヤーをページに埋め込む場合、そのコンポーネントにフォーカスした状態から、Tabキー、矢印キー、Escキーなどで抜け出すことができるようにする。
チェック内容
   *  |behavior|： 音声/動画プレイヤーにフォーカスがある状態で、Tab/Shift+Tabキー、矢印キー、Escキーのいずれかの操作で、フォーカスをプレイヤーから外すことができる。

.. raw:: html

   <div><details>

意図
````

キーボードのみを利用している場合に、ページ中の特定のコンポーネントがページの他の部分へのアクセスを阻害しないようにする。

参考
````

*  :ref:`exp-keyboard-notrap`

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 2.1.2:

   *  |SC 2.1.2|
   *  |SC 2.1.2ja|

.. raw:: html

   </div></details>


.. _multimedia-content-access:

内容へのアクセス
~~~~~~~~~~~~~~~~

参考： :ref:`exp-multimedia-content-access`

.. _gl-multimedia-text-alternative:

[MUST] テキスト情報と同等の内容にする
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] テキスト情報の代替情報として音声・映像コンテンツを用い、そのコンテンツがテキスト情報の代替であることを明示する。
チェック内容
   *  |visual|： 音声・映像コンテンツは、そのコンテンツがなくても不足なく情報が伝わるような内容で、そのコンテンツがテキスト情報の代替もしくは補助的な位置づけであることが明示されている。

.. raw:: html

   <div><details>

意図
````

音声・映像コンテンツの利用ができないユーザーも支障なくコンテンツを利用できるようにする。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.2.1:

   *  |SC 1.2.1|
   *  |SC 1.2.1ja|

*  SC 1.2.2:

   *  |SC 1.2.2|
   *  |SC 1.2.2ja|

*  SC 1.2.3:

   *  |SC 1.2.3|
   *  |SC 1.2.3ja|

*  SC 1.2.4:

   *  |SC 1.2.4|
   *  |SC 1.2.4ja|

.. raw:: html

   </div></details>

.. _gl-multimedia-caption:

[MUST] キャプションの提供
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] テキストの代替情報ではない音声・映像コンテンツにおいて、音声情報には、同期したキャプションを提供する。

   ただしライブ配信の場合は [SHOULD]

チェック内容
   *  |visual|： 音声を含むコンテンツには、同期したキャプションが提供されている。

.. raw:: html

   <div><details>

意図
````

音声情報を理解できなくてもサービスの利用が困難にならないようにする。

聴覚紹介者が、音声コンテンツおよび動画コンテンツ内の音声を理解できるようにする。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.2.2:

   *  |SC 1.2.2|
   *  |SC 1.2.2ja|

*  SC 1.2.4:

   *  |SC 1.2.4|
   *  |SC 1.2.4ja|

.. raw:: html

   </div></details>

.. _gl-multimedia-video-description:

[MUST] 音声解説の提供
^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] テキストの代替情報ではない音声・映像コンテンツにおいて、映像がある収録済みコンテンツの場合、映像の内容が分かるような同期した音声情報、またはテキストによる説明を提供する。
チェック内容
   *  |visual|： 動画は、元々収録されている音声トラックの内容から容易に映像を推測できる。または
   *  |visual|： 動画には音声解説が含まれている。または
   *  |visual|： 映像に関するテキストによる説明が提供されている。

.. raw:: html

   <div><details>

意図
````

映像情報を理解できなくてもサービスの利用が困難にならないようにする。

視覚障害者が、映像コンテンツを理解できるようにする。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.2.3:

   *  |SC 1.2.3|
   *  |SC 1.2.3ja|

.. raw:: html

   </div></details>

.. _gl-multimedia-transcript:

[MUST] 書き起こしテキストの提供
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [MUST] テキストの代替情報ではない、映像がなく音声のみの収録済みコンテンツの場合は、書き起こしテキストを提供する。
チェック内容
   *  |visual|： 映像がない音声のみのコンテンツについて、音声を書き起こしたテキストが提供されている。

.. raw:: html

   <div><details>

意図
````

音声コンテンツを理解できなくてもサービスの利用が困難にならないようにする。

聴覚障害者が音声のみのコンテンツを理解できるようにする。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.2.1:

   *  |SC 1.2.1|
   *  |SC 1.2.1ja|

.. raw:: html

   </div></details>

.. _gl-multimedia-sign-language:

[SHOULD] 手話の提供
^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [SHOULD] 収録済みコンテンツの音声情報には、同期した手話通訳を提供する。
チェック内容
   *  |visual|： 動画の音声情報には同期した手話通訳が提供されている。

.. raw:: html

   <div><details>

意図
````

手話を主たる言語として使う聴覚障害者が、音声コンテンツまたは動画コンテンツ中の音声を理解できるようにする。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.2.6:

   *  |SC 1.2.6|
   *  |SC 1.2.6ja|

.. raw:: html

   </div></details>

.. _gl-multimedia-background-sound:

[SHOULD] 充分に小さい背景音
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

ガイドライン
   [SHOULD] 映像がなく音声のみの収録済みコンテンツの場合で主たる発話音声があるとき、背景音がない、もしくは主たる発話音声に対して背景音の音量が少なくとも20db小さい状態にする。
チェック内容
   *  |visual|： 音声コンテンツについて、充分に聴き取りやすい。


.. raw:: html

   <div><details>

意図
````

音声コンテンツの内容を聞き取りやすいものにする。

対応するWCAG 2.1の達成基準
````````````````````````````

*  SC 1.4.7:

   *  |SC 1.4.7|
   *  |SC 1.4.7ja|

.. raw:: html

   </div></details>
