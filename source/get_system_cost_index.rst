.. _get_system_cost_index:

星系のコスト指数取得関数
========================

CREST経由で、特定の星系での生産活動にかかるコスト指数を返します。

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
