.. _get_income_and_expenses:

収支取得関数
============

指定期間の収入および支出を返します。

使用方法
--------
関数名::

  getIncome(from_date, to_date, character_name, wallet_division, key_id, v_code)     // 収入
  getExpenses(from_date, to_date, character_name, wallet_division, key_id, v_code)   // 支出

引数の意味
    1. 開始日付 (例: "2016/10/10" "2016/10/10 09:16:00")
    2. 終了日付
    3. キャラクター名
    4. ウォレット部門 (0から6)
    5. APIキーID
    6. API Verification Code

返り値
    数値

使用例
------
::

   =getIncome("2016/10/10", "2016/10/11", "Hirotosh Mabata", 0, "123456", "vCode")
   =getExpenses("2016/10/10", "2016/10/11", "Hirotosh Mabata", 0, "123456", "vCode")

細かな仕様
----------

* 2016/10/12現在、EVEサーバーから取得できる記録は1ヶ月ほどのようです。
