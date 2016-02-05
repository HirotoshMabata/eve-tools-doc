.. _get_market_price:

アイテム価格取得関数 (Google SpreadSheet)
=========================================

CREST経由で、特定のステーション内の注文価格を返します。
売りまたは買い、最小または最大価格を選択できます。

インストール情報
----------------
使用前の準備については :ref:`how_to_import_library` を参照してください。

プロジェクトID::

  MmmFZZTewMcpEk94vcRt5-OdSnBAmjm9N

コード::

  function getMarketPrice(a, b, c, d, e) {
    return EVEOnlineGetCRESTMarketPrice.getMarketPrice(a, b, c, d, e)
  }

使用方法
--------
関数名::

  getMarketPrice(region_id, type_id, station_name, order_string, operation_string)

引数の意味
    1. Region ID
    2. アイテムのType ID
    3. ステーション名
    4. 注文の種類: "sell" または "buy"
    5. 演算子: "min" または "max"

返り値
    数値

使用例
------
::

   =getMarketPrice(10000002, 34, "Jita IV - Moon 4 - Caldari Navy Assembly Plant", "sell", "min")

細かな仕様
----------

* ステーション名を空にすると、リージョン全体で検索します
* 注文が存在しない場合、0.00iskを返します
* CCPのサーバとの接続に失敗した場合でも、3回までリトライします

更新履歴
--------
Ver.5 2016/02/04
     初出ということで。
