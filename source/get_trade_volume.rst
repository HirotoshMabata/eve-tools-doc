.. _get_trade_volume:

取引量取得関数
==============

CREST経由で、アイテムの取引量を返します。

使用方法
--------
関数名::

  getTradeVolume(region_id, type_id, operation_string)

引数の意味
    1. Region ID
    2. Type ID
    3. 演算子

       * "latest": 最新の取引量を返します
       * "average": 取得できた取引量をすべて平均したものを返します。Ver.1現在で、2015年01月01日からの平均を返します。

返り値
    数値

使用例
------
::

   =getTradeVolume(10000002, 34, "latest")

細かな仕様
----------

* CCPのサーバとの接続に失敗した場合でも、3回までリトライします
* 取引がない場合は 0.0 を返します
