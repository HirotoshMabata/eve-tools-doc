.. _get_market_stock:

在庫取得関数
============

CREST経由で、特定のステーション内の総在庫数を返します。
売りまたは買いを選択できます。

使用方法
--------
関数名::

  getMarketStock(region_id, type_id, station_name, order_string)

引数の意味
    1. Region ID
    2. アイテムのType ID
    3. ステーション名
    4. 注文の種類: "sell" または "buy"

返り値
    数値

使用例
------
::

   =getMarketStock(10000002, 34, "Jita IV - Moon 4 - Caldari Navy Assembly Plant", "sell")

細かな仕様
----------

* ステーション名を空にすると、リージョン全体で検索します
