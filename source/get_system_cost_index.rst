.. _get_system_cost_index:

星系のコスト指数取得関数 (Google SpreadSheet)
=============================================

CREST経由で、特定の星系での生産活動にかかるコスト指数を返します。

インストール情報
----------------
使用前の準備については :ref:`how_to_import_library` を参照してください。

プロジェクトID::

  MvWLo01ttq_6TKr5i7fE2H-dSnBAmjm9N

コード::

  function getSystemCostIndex(a,b) {
    return EVESystemCostIndex.getSystemCostIndex(a,b)
  }

使用方法
--------
関数名::

  getSystemCostIndex(system_name, activity_name)

引数の意味
    1. 星系の名前
    2. アクティビティ名：以下のいずれか

       * "Invention"
       * "Manufacturing"
       * "Researching Time Efficiency"
       * "Researching Material Efficiency"
       * "Copying"

返り値
    数値

使用例
------
::

   =getSystemCostIndex("Jita", "Manufacturing")

細かな仕様
----------

* CCPのサーバとの接続に失敗した場合でも、3回までリトライします

更新履歴
--------
Ver.2 2016/02/03
     初出ということで。
