.. _get_adjusted_price:

Adjusted Price取得関数
======================

CREST経由で、生産のジョブコスト算出に使われる「Adjusted Price」を返します。

使用方法
--------
関数名::

  getAdjustedPrice(type_id)

引数の意味
    1. アイテムのType ID

返り値
    数値

使用例
------
::

   =getAdjustedPrice(43)

細かな仕様
----------

* CCPのサーバとの接続に失敗した場合でも、3回までリトライします
