# シゴトミル 職業データ（37業界・320職業）

> **English**: Japanese occupational interest (RIASEC-type, 6 domains) and work-value (11 items) data for 37 industries and 320 occupations, derived from the "job tag" (Japanese O-NET) public dataset by MHLW / JILPT, ver. 7.00. CSV and JSON. Industry grouping and slugs were added by Shigotomiru (https://tekishoku-compass.com/dataset/). Use under Article 9 of the job tag Terms of Use with attribution — see [LICENSE.md](LICENSE.md).

厚生労働省の職業情報提供サイト「job tag（日本版O-NET）」の公開データを、**37業界**と**320職業**の単位で並べ直した数値です。
サイト [シゴトミル](https://tekishoku-compass.com/) の記事と診断が使っているものと同じファイルを、そのまま置いています。

配布ページ（列の意味・使うときの条件の正本）: **https://tekishoku-compass.com/dataset/**

## ファイル

| | 業界版 | 職業版 |
|---|---|---|
| 行 | 37業界（業界平均） | 320職業 |
| 列 | 6つの興味の向き | 6つの興味の向き＋仕事で大事にしている11項目 |
| CSV | [data/industries.csv](data/industries.csv) | [data/jobs.csv](data/jobs.csv) |
| JSON | [data/industries.json](data/industries.json) | [data/jobs.json](data/jobs.json) |

CSV の先頭6行は `#` で始まるコメント（出典・範囲・尺度・ライセンス・列・配布元）です。数値だけ欲しいときは読み飛ばしてください。

## 列の意味（要約）

- **6つの興味の向き**（1.00〜5.00。高いほどその向きが強い）: `realistic`（現実的）/ `investigative`（研究的）/ `artistic`（芸術的）/ `social`（社会的）/ `enterprising`（企業的）/ `conventional`（慣習的）
- **仕事で大事にしている11項目**（職業版だけ。1.00〜5.00）: 達成感・自律性・専門性・自己成長・社会的認知・奉仕貢献・対人関係・労働安全・私生活・雇用安定・報酬。その仕事をしている人が何をどれだけ大事にしているかの値で、給与額・労働時間・安全性そのものではありません。列名はシゴトミルの略記です（原語の対応は [配布ページ](https://tekishoku-compass.com/dataset/)）
- `slug` と `industry`（37業界の分類）はシゴトミルが付けたもので、job tag にはありません

## 使うときの条件

job tag の利用規約（第9条）は、編集・加工・再集計などの二次利用を認めています。条件は**出典の表示**です。次の形で書けば足ります。

> 出典：シゴトミル「データのダウンロード」（https://tekishoku-compass.com/dataset/）／原データ：厚生労働省 職業情報提供サイト（日本版O-NET）「job tag」簡易版数値系ダウンロードデータ ver.7.00（https://shigoto.mhlw.go.jp/User/download　2026年8月13日取得／制作・著作：独立行政法人 労働政策研究・研修機構）

ファイルに入っているのは数値と職業名だけです。job tag の設問文は入れていません（利用規約 第8条）。

## もとのデータ

- 出典：厚生労働省 職業情報提供サイト（日本版O-NET）[「job tag」簡易版数値系ダウンロードデータ ver.7.00](https://shigoto.mhlw.go.jp/User/download)（最終更新 2026年3月17日／制作・著作：独立行政法人 労働政策研究・研修機構）
- 取得日：2026年8月13日
- 業界平均の作り方、1職業あたりの回答数、この数値で分かること：[このサイトのデータについて](https://tekishoku-compass.com/method/)

## 更新

URL とファイル名は固定です。job tag が更新されたら、このリポジトリと配布ページを同時に更新します。バージョンはファイルの中に書いてあります。
