.. _get_skill_level:

スキルレベル取得関数
====================

APIキーを使用して、キャラクターのスキルレベルを取得する関数です。

使用方法
--------

関数名::

  getSkillLevel(key, vCode, characterID, skillTypeID)

引数の意味
    1. APIキー
    2. APIコード
    3. キャラクターID
    4. スキルのType ID

返り値
    数値

使用例
------
::

   =getSkillLevel(12345678, "asdkfjafaksjhfasdj...", 09876543, 3386)
