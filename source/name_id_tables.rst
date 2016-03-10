.. _name_id_tables:

名前とIDの対応表
================

Google SpreadSheetで名前・ID対応表を作ってみました。

* `アイテム名 - TypeID (Ver. YC-118-3) <https://docs.google.com/spreadsheets/d/1J_PlvzKflT8Zp1_xJ6m1ZyQJh2378ZP_HyPr-hyqHaQ/edit?usp=sharing>`_
* `ソーラーシステム名 - システムID (Ver. YC-118) <https://docs.google.com/spreadsheets/d/1GjrEeSx2Nx_Q-6OnLTvXDub_cFubxoxaShgaVf611MY/edit?usp=sharing>`_
* `ステーション名 - ステーションID (Ver. YC-118) <https://docs.google.com/spreadsheets/d/150D4RRjwKrAtnKA1RP0sxScvAE20ITGBH3Bvyv8zmNc/edit?usp=sharing>`_
* `リージョン名 - リージョンID <https://docs.google.com/spreadsheets/d/1OM2L8j6lSppc7IxWWhxEN_JgfwlqiCJFWoU0pWz7FzA/edit?usp=sharing>`_

利用するには、表をコピペするか、次のような数式をセルに入れるとよさげです。 ::

  =importrange("https://docs.google.com/spreadsheets/d/1J_PlvzKflT8Zp1_xJ6m1ZyQJh2378ZP_HyPr-hyqHaQ/edit?usp=sharing","A:B")

URLの部分を、利用したい表のURLに置き換えてください。
