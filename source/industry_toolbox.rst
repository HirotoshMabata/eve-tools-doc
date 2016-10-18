.. _industry_toolbox:

Industry Toolbox
================

Googleスプレッドシート向けのマーケット情報を取得する関数群です。

現在は以下の関数を提供しています。

.. toctree::
   :maxdepth: 1

   get_adjusted_price
   get_market_price
   get_system_cost_index
   get_trade_volume
   get_character_names
   character_name_to_id
   get_skill_level
   get_implants
   get_market_stock
   get_market_history

インストール方法
----------------

1. スクリプトエディタを開く

.. image:: ../images/open_script_editor.png

2. ライブラリを開く

.. image:: ../images/open_library.png

3. プロジェクトを適当な名前で保存する

.. image:: ../images/save_project.png

4. 以下のプロジェクトIDを「ライブラリを検索」テキストボックスへ入れる ::

     MjKqKwe6OLi5o2AN_V8dH7pBOPJZB1Egd

5. 最新のバージョンを選択する

.. image:: ../images/select_version.png

6. 以下のコードをコピペして保存する。 ::

     function getMarketPrice(region_id, type_id, station_string, sell_or_buy_string, min_or_max_string, refresh_code) {
       return EVEIndustryToolbox.getMarketPrice(region_id, type_id, station_string, sell_or_buy_string, min_or_max_string, refresh_code)
     }

     function getAdjustedPrice(type_id, refresh_code) {
       return EVEIndustryToolbox.getAdjustedPrice(type_id)
     }

     function getTradeVolume(region_id, type_id, operation_string, refresh_code) {
       return EVEIndustryToolbox.getTradeVolume(region_id, type_id, operation_string)
     }

     function getSystemCostIndex(system_name, activity_name, refresh_code) {
       return EVEIndustryToolbox.getSystemCostIndex(system_name, activity_name)
     }

     function getCharacterNames(key, vCode, refresh_code) {
       return EVEIndustryToolbox.getCharacterNames(key, vCode)
     }

     function characterNameToID(name, refresh_code) {
       return EVEIndustryToolbox.characterNameToID(name)
     }

     function getSkillLevel(key, vCode, characterID, skillTypeID, refresh_code) {
       return EVEIndustryToolbox.getSkillLevel(key, vCode, characterID, skillTypeID)
     }

     function getImplants(key, vCode, characterID, refresh_code) {
       return EVEIndustryToolbox.getImplants(key, vCode, characterID)
     }

     function getMarketStock(region_id, type_id, station_name, order_string, refresh_code) {
       return EVEIndustryToolbox.getMarketStock(region_id, type_id, station_name, order_string)
     }

     function getMarketHistory(region_id, type_id, refresh_code) {
       return EVEIndustryToolbox.getMarketHistory(region_id, type_id)
     }

     function onOpen() {
       EVEIndustryToolbox.onOpen()
     }

     function showRequestCount() {
       EVEIndustryToolbox.showRequestCount()
     }

以上で準備完了です。

アップデート方法
----------------

1. 最新のバージョンを選択しなおす

.. image:: ../images/select_version.png

2. 上記のコードをコピペしなおして保存する

以上でアップデート完了です。

更新履歴
--------
Ver.9 2016/10/18
    GetTradeVolume関数に7日間/30日間平均を追加

Ver.8 2016/06/27
    GetMarketHistory関数を追加

Ver.7 2016/06/14
    CCP側のCREST仕様変更に対応

Ver.6 2016/05/21
    public-crest.eveonline.comからcrest-tq.eveonline.comへ移行

Ver.5 2016/03/10
    getMarketStock関数を追加

Ver.4 2016/02/15
    getImplants関数を追加

Ver.3 2016/02/13
    getSkillLevel関数: スキルを覚えていない場合は 0 を返すよう修正

Ver.2 2016/02/13
    getCharacterNames, characterNameToID, getSkillLevel関数を追加

Ver.1 2016/02/12
    初出ということで。
