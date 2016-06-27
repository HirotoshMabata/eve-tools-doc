.. _get_market_history:

マーケット取引履歴取得関数
============

CREST経由で、特定リージョンのアイテム取引履歴を取得します。

使用方法
--------
関数名::

  getMarketHistory(region_id, type_id)

引数の意味
    1. Region ID
    2. アイテムのType ID

返り値
    日付、注文数、取引量、最低価格、最高価格、平均価格の配列

使用例
------
::

   =getMarketHistory(10000002, 34)
