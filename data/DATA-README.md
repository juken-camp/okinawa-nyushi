# 沖縄県立高校・学校別入試情報データベース 最終版

バージョン: 9.0.0-final  
基準日: 2026-07-07

## 完了状態

`complete_with_documented_unresolved`

全59校・164学科／コースを収録し、公式資料で確認できた情報を構造化しています。公式未公表、公式資料を発見できない項目、外部サーバー障害により全文確認できない項目は、推測せず状態値と `unresolved-items.csv/json` に記録しています。

## 年度

令和9年度の学校別募集要項・特色選抜資料は、元資料上2026年7月7日時点で未公表です。全164レコードは令和8年度公式資料を前年度参考として収録しています。

## 外部資料の確認例外

- `koza-f`
- `okisui-kg`
- `okisui-ks`
- `okisui-sg`

上記4レコードは、公式PDFの所在・検索索引本文は確認済みですが、PDF本体の502エラーにより全セルを確認できず、`school_detail_partial` としています。確認できた配点・資格級・主要ランクのみ収録し、未確認部分は補完していません。

`koza-night-commerce` は別区分です。令和8年度の実績ランク表を確認できず、取得できた令和7年度表は過年度参考として分離管理しています。

## 主なファイル

- `admission-details.json` / `.csv` / `.js`
- `achievement-ranks.json` / `.js`
- `sources.csv` / `.json` / `.js`
- `school-id-map.csv`
- `unresolved-items.csv` / `.json`
- `data-validation-report.md`
- `research-summary.md`
- `research-manifest.json`
- `legacy-program-data.json`

`legacy-program-data.json` は、統合前サイトに存在したものの、現行公式母集団では廃止・再編・分割扱いとなった旧8IDの追跡調査データです。現行学科へ推測転用せず分離保存しています。

## 令和9年度公開後

令和9年度の学校別資料が公表されたら、`previous_reference` の令和8年度レコードを、出典単位で令和9年度版へ差し替えてください。

第三者監査の詳細はルートの `AUDIT-REPORT.md` を参照してください。元資料由来の主要JSON・CSV・検証資料本体は変更していません。
