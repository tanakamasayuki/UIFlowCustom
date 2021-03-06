# UIFlowCustom
UIFlowのカスタムブロックを公開しています。

## 天気予報

気象庁の公開しているJSONデータを読み込んで、今日と明日、明後日の天気予報情報を取得します。

天気予報取得ブロックに取得する地域コードを指定してください。

https://www.jma.go.jp/bosai/#area_type=offices&area_code=130000

この番号は気象庁の天気を表示するときのURLの最後についている数値と同じです。参考のため、地域選択のページで表示されているものを一覧にしてみました。青森県の場合には020000にすることで天気予報のデータを取得可能です。離島などの場合は気象庁のページより該当部分を表示して、URLよりコードを確認してみてください。

| エリア               | 地域                     | コード |
|----------------------|--------------------------|--------|
| 北海道               | 宗谷地方                 | 011000 |
| 北海道               | 上川・留萌地方           | 012000 |
| 北海道               | 網走・北見・紋別地方     | 013000 |
| 北海道               | 十勝地方                 | 014030 |
| 北海道               | 釧路・根室地方           | 014100 |
| 北海道               | 胆振・日高地方           | 015000 |
| 北海道               | 石狩・空知・後志地方     | 016000 |
| 北海道               | 渡島・檜山地方           | 017000 |
| 東北                 | 青森県                   | 020000 |
| 東北                 | 岩手県                   | 030000 |
| 東北                 | 宮城県                   | 040000 |
| 東北                 | 秋田県                   | 050000 |
| 東北                 | 山形県                   | 060000 |
| 東北                 | 福島県                   | 070000 |
| 関東甲信             | 茨城県                   | 080000 |
| 関東甲信             | 栃木県                   | 090000 |
| 関東甲信             | 群馬県                   | 100000 |
| 関東甲信             | 埼玉県                   | 110000 |
| 関東甲信             | 千葉県                   | 120000 |
| 関東甲信             | 東京都                   | 130000 |
| 関東甲信             | 神奈川県                 | 140000 |
| 関東甲信             | 山梨県                   | 190000 |
| 関東甲信             | 長野県                   | 200000 |
| 北陸                 | 新潟県                   | 150000 |
| 北陸                 | 富山県                   | 160000 |
| 北陸                 | 石川県                   | 170000 |
| 北陸                 | 福井県                   | 180000 |
| 東海                 | 岐阜県                   | 210000 |
| 東海                 | 静岡県                   | 220000 |
| 東海                 | 愛知県                   | 230000 |
| 東海                 | 三重県                   | 240000 |
| 近畿                 | 滋賀県                   | 250000 |
| 近畿                 | 京都府                   | 260000 |
| 近畿                 | 大阪府                   | 270000 |
| 近畿                 | 兵庫県                   | 280000 |
| 近畿                 | 奈良県                   | 290000 |
| 近畿                 | 和歌山県                 | 300000 |
| 中国(山口を除く)     | 鳥取県                   | 310000 |
| 中国(山口を除く)     | 島根県                   | 320000 |
| 中国(山口を除く)     | 岡山県                   | 330000 |
| 中国(山口を除く)     | 広島県                   | 340000 |
| 四国                 | 徳島県                   | 360000 |
| 四国                 | 香川県                   | 370000 |
| 四国                 | 愛媛県                   | 380000 |
| 四国                 | 高知県                   | 390000 |
| 九州北部(山口を含む) | 山口県                   | 350000 |
| 九州北部(山口を含む) | 福岡県                   | 400000 |
| 九州北部(山口を含む) | 佐賀県                   | 410000 |
| 九州北部(山口を含む) | 長崎県                   | 420000 |
| 九州北部(山口を含む) | 熊本県                   | 430000 |
| 九州北部(山口を含む) | 大分県                   | 440000 |
| 九州南部・奄美       | 宮崎県                   | 450000 |
| 九州南部・奄美       | 鹿児島県（奄美地方除く） | 460100 |
| 九州南部・奄美       | 奄美地方                 | 460040 |
| 沖縄                 | 沖縄本島地方             | 471000 |
| 沖縄                 | 大東島地方               | 472000 |
| 沖縄                 | 宮古島地方               | 473000 |
| 沖縄                 | 八重山地方               | 474000 |

