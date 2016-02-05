.. _get_adjusted_price:

Adjusted Price取得関数 (Google SpreadSheet)
===========================================

CREST経由で、生産のジョブコスト算出に使われる「Adjusted Price」を返します。

インストール情報
----------------
使用前の準備については :ref:`how_to_import_library` を参照してください。

プロジェクトID::

  M_2APPpTCsPs7VyQD2NROtOdSnBAmjm9N

コード::

  function getAdjustedPrice(a) {
    return EVEAdjustedPrice.getAdjustedPrice(a)
  }

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

更新履歴
--------
Ver.1 2016/02/04
     初出
