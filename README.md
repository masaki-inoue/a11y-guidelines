# freee Accessibility Guidelines

freee株式会社が作成しているアクセシビリティー・ガイドラインの一般公開版のリポジトリーです。現在作成中で、随時更新する予定です。

このガイドラインの作成の経緯などについて詳しくは、[ガイドラインのイントロダクション](https://a11y-guidelines.freee.co.jp/intro/index.html)と、[freee Developers Blogの記事](https://developers.freee.co.jp/entry/a11y-guidelines-202004.0)をご覧ください。

## 最新ファイルの入手

以下のURLで最新のファイルを入手していただけます:

* HTML版: <https://a11y-guidelines.freee.co.jp/>
* HTMLファイルをまとめたzipファイルおよびソースファイル: <https://github.com/freee/a11y-guidelines/releases/latest>

## この文書に関するお問い合わせなど

この文書に関するお問い合わせ、ご意見などは、このリポジトリーでissueを作成してお知らせください。

誤字脱字の修正など、エディトリアルな修正の提案については、issueまたはpull requestを作成してください。

## 日本語の表記ルールについて

このガイドラインは、 原則として[日本翻訳連盟](https://www.jtf.jp/)が公開している[JTF日本語標準スタイルガイド(翻訳用）](https://www.jtf.jp/jp/style_guide/styleguide_top.html)に従って記述しています。

リポジトリーのルート・ディレクトリーの `.textlintrc` に、現在使用しているtextlintのルールが含まれていますが、現時点では不完全な状態です。

## ソースについて

この文書はreStructuredTextで記述し、Sphinxで処理しています。
HTMLファイルの生成には、Python 3.x (開発環境では3.7.xを使っています)、[Sphinx](https://www.sphinx-doc.org/en/master/)と[Read the Docs Sphinx Theme (sphinx_rtd_theme)](https://github.com/readthedocs/sphinx_rtd_theme)が必要です。

このリポジトリーをcloneしたうえで、Pythonが利用できる環境で、以下のように実行するとHTMLを生成することができます:

`````
% pip install --upgrade pip
% pip install -r requirements.txt
% make html
`````

## ライセンス

![クリエイティブ・コモンズ・ライセンス](https://i.creativecommons.org/l/by/4.0/88x31.png)
「freeeアクセシビリティー・ガイドライン」は、freee株式会社が作成したもので、[クリエイティブ・コモンズ 表示 4.0 国際 ライセンス](http://creativecommons.org/licenses/by/4.0/)で提供されています。

Copyright © 2020, freee株式会社

## 更新履歴

### 次期リリース

* 誤字修正 ([#10](https://github.com/freee/a11y-guidelines/pull/10), [#11](https://github.com/freee/a11y-guidelines/pull/11))

### [Ver. 202007.0](https://github.com/freee/a11y-guidelines/releases/202007.0/) (2020年7月10日)

* 参考情報追加：[スクリーン・リーダーを用いたチェックの実施方法](https://a11y-guidelines.freee.co.jp/explanations/screen-reader-check.html#exp-screen-reader-check)
* 参考情報更新
  - [様々なユーザーの入力手段の特徴とそのサポート](https://a11y-guidelines.freee.co.jp/explanations/input_device-various.html#exp-input-device-various)：[[MUST] ダウン・イベントをトリガーにしない](https://a11y-guidelines.freee.co.jp/categories/input_device.html#gl-input-device-use-up-event)に関する説明で、クリック・イベントについての記述を追加
* 動的コンテンツの[[MUST] 点滅、スクロールを伴うコンテンツ](https://a11y-guidelines.freee.co.jp/categories/dynamic_content.html#gl-dynamic-content-pause-movement)から「動きを伴うコンテンツ」の記述を削除し、音声・映像コンテンツにアニメーションや動画を対象とした新ガイドラインを追加：[[MUST] 動きを伴うコンテンツ](https://a11y-guidelines.freee.co.jp/categories/multimedia.html#gl-multimedia-pause-movement)
* リンクのターゲット・サイズに関するガイドラインについて、テキスト・リンクについてはWCAGで例外とされているので、アイコンの場合の基準のみ記し、アイコンのカテゴリーに移動：[[SHOULD] 十分な大きさのクリック/タッチのターゲット](https://a11y-guidelines.freee.co.jp/categories/icon.html#gl-icon-target-size)
* フォームのターゲット・サイズに関するガイドラインについて、アイコンと同じ基準を明記：[[SHOULD] 十分な大きさのクリック/タッチのターゲット](https://a11y-guidelines.freee.co.jp/categories/form.html#gl-form-target-size)
* 入力ディバイスのガイドライン2項目をマージ：[[MUST] 特定の入力ディバイスを前提としない](https://a11y-guidelines.freee.co.jp/categories/input_device.html#gl-input-device-independent)
  マージ対象ガイドライン：
  - [MUST] 入力ディバイスのサポート：OSがサポートしている入力ディバイスの使用を妨げない。
  - [MUST] ユーザーの動きだけをトリガーにしない：加速度センサー、モーション・キャプチャーなどを活用した、ユーザーの動きをトリガーにする機能は、他のインターフェースによっても実行できるようにする。
* ガイドラインの文言を一部変更（下表参照）

#### Ver. 202007.0でのガイドライン文言変更箇所

| 該当箇所 | 変更前 | 変更後 | 補足 |
|---|---|---|---|
| ページ全体：[[SHOULD] 適切なセクション分けと見出しの付与](https://a11y-guidelines.freee.co.jp/categories/page.html#gl-page-headings) |  `h?` 要素を使って適切に見出しを付ける。 |  コンテンツを適切にセクション分けし、 `h?` 要素を使って見出しを付ける。 |  意図が明確になるように同ガイドラインの見出しも変更しています。 |
| 入力ディバイス：[[MUST] ダウン・イベントをトリガーにしない](https://a11y-guidelines.freee.co.jp/categories/input_device.html#gl-input-device-use-up-event) |  操作の実行、完了のトリガーにはダウン・イベントを使わず、アップ・イベントを使う。 |  クリックやタップで実行される機能の実行、完了のトリガーには、ダウン・イベントを使わず、アップ・イベントやクリック・イベントを使い、誤った操作を中断できるようにする。 |  意図の項にも追記して、ドラッグ&amp;ドロップがこのガイドラインに抵触しないことを明示しています。 |
| テキスト：[[MUST] 適切な文言の見出し](https://a11y-guidelines.freee.co.jp/categories/text.html#gl-text-heading-label) |  主題又は目的を説明する見出しおよびラベルを付ける。 |  主題又は目的を説明する見出しを付ける。 |  「ラベル」はフォーム・コントロールと画像の説明を意図したものでしたが、これらはそれぞれ別カテゴリーでカバーされているため削除しました。併せて見出しも変更しています。 |
| テキスト：[[MUST] 複数の視覚的要素を用いた表現](https://a11y-guidelines.freee.co.jp/categories/text.html#gl-text-color-only) |  文字色に何らかの意味を持たせている場合、書体など他の視覚的な要素も併せて用い、色が判別できなくてもその意味を理解できるようにする。 |  強調、引用など、何らかの意図を文字色を変えることによって表現している場合、書体など他の視覚的な要素も併せて用い、色が判別できなくてもその意味を理解できるようにする。 |  ガイドラインの意図を考慮して、掲載セクションを変更しています。 |
| 音声・映像コンテンツ：[[MUST] 書き起こしテキストの提供](https://a11y-guidelines.freee.co.jp/categories/multimedia.html#gl-multimedia-transcript) |  テキストの代替情報ではない音声・映像コンテンツにおいて、映像がなく音声のみの収録済みコンテンツの場合は、書き起こしテキストを提供する。 |  テキストの代替情報ではない、映像がなく音声のみの収録済みコンテンツの場合は、書き起こしテキストを提供する。 | |
| 動的コンテンツ：[[MUST] 点滅、スクロールを伴うコンテンツ](https://a11y-guidelines.freee.co.jp/categories/dynamic_content.html#gl-dynamic-content-pause-movement) |  自動的に開始し5秒以上継続する、点滅、スクロールまたは動きを伴うコンテンツを作らない。そのようなコンテンツを作る場合は、ユーザーが一時停止、停止、非表示にすることができるようにする。 |  同じページ上に、自動的に開始し5秒以上継続する、点滅やスクロールを伴うコンテンツと、他のコンテンツを一緒に配置しない。そのようなコンテンツを作る場合は、ユーザーが一時停止、停止、または非表示にすることができるようにする。 | |
| 動的コンテンツ：[[MUST] 自動更新されるコンテンツ](https://a11y-guidelines.freee.co.jp/categories/dynamic_content.html#gl-dynamic-content-pause-refresh) |  自動的に内容が更新されるコンテンツを作らない。そのようなコンテンツを作る場合は、ユーザーが一時停止、停止、非表示にすることができるか、更新頻度を調整できるようにする。 |  予め設定された間隔で自動的に内容が更新されたり非表示になったりするコンテンツを作らない。そのようなコンテンツを作る場合は、ユーザーが一時停止、停止、非表示にすることができるか、更新頻度を調整できるようにする。 | |
| フォーム：[[SHOULD] 誤操作の防止](https://a11y-guidelines.freee.co.jp/categories/form.html#gl-form-errors-cancel) |  誤った操作が確定することでユーザーに不利益が生じる可能性がある機能については、取り消し、送信前の確認・修正、または送信時のエラー・チェックと修正を可能にする。 |  法的行為、経済的取引、データの変更や削除を生じる機能については、取り消し、送信前の確認・修正、または送信時のエラー・チェックと修正を可能にする。 | |


### [Ver. 202006.0](https://github.com/freee/a11y-guidelines/releases/202006.0/) (2020年6月18日)

* ガイドライン部分の文書構造を見直し
* [入力ディバイス](http://a11y-guidelines.freee.co.jp/categories/input_device.html)に関するガイドラインの構成を一部変更（内容に変更無し）
* コントラスト関連のガイドラインで、文字サイズの表記をpxとptを併記するように変更
* [動的コンテンツ](http://a11y-guidelines.freee.co.jp/categories/dynamic_content.html)に関するガイドラインにガイドラインを1項目追加： [[MUST] 適切なDOMツリーを維持する](http://a11y-guidelines.freee.co.jp/categories/dynamic_content.html#gl-dynamic-content-maintain-dom-tree)
* その他内容の変更を伴わないガイドライン文言の変更
* 「チェック内容」と「チェック対象」を対にして表記するように変更
* チェック内容の追加と文言変更
* 「意図」について、一部内容の変更を伴わない文言変更と追記

### [Ver. 202005.1](https://github.com/freee/a11y-guidelines/releases/202005.1/) (2020年5月26日)

* [日本翻訳連盟](https://www.jtf.jp/)が公開している[JTF日本語標準スタイルガイド(翻訳用）](https://www.jtf.jp/jp/style_guide/styleguide_top.html)に基づき表記揺れなど修正 ([#7](https://github.com/freee/a11y-guidelines/issues/7))
* 誤字修正

### [Ver. 202005.0](https://github.com/freee/a11y-guidelines/releases/202005.0/) (2020年5月21日、Global Accessibility Awareness Day)

* 一部文言を修正
* 色に関するガイドラインについて、色弱者に加えて視覚障害者のアクセスに影響することを「意図」に明記
* 参考情報の追加:
    - [自動的に変化するコンテンツの問題点](https://a11y-guidelines.freee.co.jp/explanations/dynamic_content-auto-updated.html)
    - [フォーム・コントロールのラベル付けの必要性](https://a11y-guidelines.freee.co.jp/explanations/form-labeling.html)
    - [色を用いた表現に関する注意点](https://a11y-guidelines.freee.co.jp/explanations/color-only.html)
    - [フォーム操作で発生する動的な変化が及ぼす影響](https://a11y-guidelines.freee.co.jp/explanations/form-dynamic-content.html)
    - [入力エラーの扱い](https://a11y-guidelines.freee.co.jp/explanations/form-errors.html)
    - [小さすぎるクリックやタッチのターゲット・サイズの問題点](https://a11y-guidelines.freee.co.jp/explanations/target-size.html#exp-target-size)
    - [画像化されたテキストの問題点](https://a11y-guidelines.freee.co.jp/explanations/images_of_text-usage.html)
    - [画像化されたテキストを使用する場合の代替情報の提供](https://a11y-guidelines.freee.co.jp/explanations/images_of_text-text-alternative.html)
    - [コントラスト比確保の重要性](https://a11y-guidelines.freee.co.jp/explanations/contrast.html)
    - [ユーザーCSSを適用したチェックの実施方法](https://a11y-guidelines.freee.co.jp/explanations/text-custom-css.html)
    - [キーボード・トラップが引き起こす問題](https://a11y-guidelines.freee.co.jp/explanations/keyboard-notrap.html)
    - [様々なユーザーの入力手段の特徴とそのサポート](https://a11y-guidelines.freee.co.jp/explanations/input_device-various.html)
    - [音声・映像コンテンツの存在を認知可能にする](https://a11y-guidelines.freee.co.jp/explanations/multimedia-perceivable.html)
    - [音声の自動再生とアクセシビリティー](https://a11y-guidelines.freee.co.jp/explanations/multimedia-autoplay.html)
    - [音声・映像コンテンツのアクセシビリティーを確保する](https://a11y-guidelines.freee.co.jp/explanations/multimedia-content-access.html)
    - [Tab/Shift+Tabキーを用いたチェック](https://a11y-guidelines.freee.co.jp/explanations/tab-order-check.html)
* 参考情報の更新:
    - [Reactコンポーネントなどのアクセシビリティー](https://a11y-guidelines.freee.co.jp/explanations/markup-component.html): AccessibleNameとroleについて加筆
* 誤字修正 ([#3](https://github.com/freee/a11y-guidelines/pull/3), [#5](https://github.com/freee/a11y-guidelines/pull/5), [#6](https://github.com/freee/a11y-guidelines/pull/6), 他)
* CSSなど修正

### [Ver. 202004.0](https://github.com/freee/a11y-guidelines/releases/202004.0/) (2020年4月30日)

* 初版公開
