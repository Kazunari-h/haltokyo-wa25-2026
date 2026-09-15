# 解答一覧（主催者用・ネタバレ注意）

各ファイルに仕込んだ不具合の一覧です。参加者には見せないでください。

| No. | ファイル | 仕込んだ不具合 |
| --- | --- | --- |
| 01 | 01-index.html | 見出しの誤字「ようこそそ」／営業時間が2つ書かれていて矛盾／ナビの「メニュー」が存在しない `menu.html` へのリンク |
| 02 | 02-about.html | 画像に `alt` がない／画像パス `images/store-front.jpg` が存在せず表示されない／電話番号が桁不足（03-1234-567） |
| 03 | 03-contact.html | 必須項目に `required` がない／メール欄が `type="text"`／送信ボタンが `type="button"` で何も起きない |
| 04 | 04-news.html | 「新しい順」と書いてあるのに日付順になっていない／3件目の表示年が2025で `datetime` の2026と不一致 |
| 05 | 05-login.html | パスワード欄が `type="text"` で入力が丸見え／エラーメッセージに正解のパスワードが表示されている |
| 06 | 06-faq.html | 3問目の `data-target="a4"` と回答の `id="a3"` が不一致でクリックしても開かない（コンソールにエラー） |
| 07 | 07-pricing.html | 価格と個数が文字列連結される（`"1000"+"1"`＝10001）／税率が1.08で見出しの10%と不一致 |
| 08 | 08-gallery.html | 2枚目の画像が1枚目と同じ（キャプションと不一致、altも違う）／6枚目の `src` が `htps://` で壊れている |
| 09 | 09-counter.html | 「+」で減り「−」で増える（逆）／0未満に下がる／リセットが画面に反映されない |
| 10 | 10-todo.html | 空欄でも追加できる／削除ボタンが `removeChild(del)` で `li` を消しておらずエラーになる／追加後に入力欄がクリアされない |
| 11 | 11-schedule.html | ヘッダーが3列なのに本文が4列（備考列の見出しがない）／火曜の `colspan="2"` でさらに列ずれ／木曜の開店と閉店が逆 |
| 12 | 12-profile.html | カードが白背景に白文字で読めない／タグも背景と文字色がほぼ同じで読めない |
| 13 | 13-search.html | 条件が逆で、キーワードに一致するものが消え、一致しないものが残る |
| 14 | 14-footer.html | コピーライトが2020年、店名が「Caffe」と誤字／Facebookのリンク先がInstagram／`privacy.html` が存在しない |
| 15 | 15-map.html | 「新しいタブで開きます」と書いてあるのに `target="_blank"` がない／逆に別リンクには `rel="noopener"` なしの `_blank`／駐車場の記述が矛盾 |
| 16 | 16-signup.html | `if (pw = pw2)` が代入になっていて、不一致でも「登録完了」になる |
| 17 | 17-timer.html | `setInterval` が500msで2倍速／スタート連打で複数タイマーが走る |
| 18 | 18-dark-mode.html | `classList.add` なので一度ダークにすると戻らない／ボタン文言も戻らない |
| 19 | 19-lang.html | `<meta charset>` がなく文字化けの可能性／英語ページなのに末尾に日本語の段落が残っている |
| 20 | 20-responsive.html | viewport meta がない／`.container` が `width:1200px` 固定／`.col` に `min-width:380px` でスマホで横スクロール |
| 21 | 21-clock.html | `</head>` が `</body>` になっている／月が `getMonth()` のままで1少ない／ゼロ埋めがなく「9:5:3」と表示 |
| 22 | 22-quiz.html | 正解判定の文字列が `'brasil'`（`brazil` ではない）で、正解のブラジルを選んでも不正解になる |
| 23 | 23-cart.html | 合計に数量が掛けられていない（`total += price`）／`input` イベントでなく `change` なので入力途中に更新されない |
| 24 | 24-accessibility.html | ボタンが `div` でTabキーで到達できない／`label` がなく入力欄と項目名が紐づいていない／`alert` を使用 |
| 25 | 25-events.html | `id="highlight"` が重複／見出しが h1→h4 に飛んでいる／目次の `#live` リンク先が `id="live-music"` で飛ばない |
| 26 | 26-download.html | 「季節限定メニュー」のリンク先が「メニュー表」と同じ／パーティープランが `.docx` なのにPDF表記／`downlaod` の誤字／`docs/` が存在しない |
| 27 | 27-modal.html | `getElementById('colse')` の誤字でモーダルが閉じられない（コンソールにエラー） |
| 28 | 28-tabs.html | 「フード」タブの `data-panel` が `sweets` になっていてスイーツが表示される |
| 29 | 29-rating.html | `i <= value` で1つ多く点灯する（星3を押すと4つ光る） |
| 30 | 30-weather.html | 気温が華氏(77)なのに℃表記／`humidty` の誤字で湿度が `undefined`／テラス席の判定が逆（雨なしで「利用不可」） |
