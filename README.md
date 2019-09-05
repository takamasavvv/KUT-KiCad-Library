# KUT-KiCad-Library

日本にない大学のrobotやらrocketの周辺に出没するKicadライブラリ

## 概要

某大学の某rocket団体とか某robot団体で使われているフリーEDA「KiCad」のライブラリを集めて煮込んだもの  
おそらく見たことある部品で固めてあるよ  
プルリク歓迎、使うならライブラリの整備協力してくれるとありがたい  
（利用は自己責任）

## 使い方

### 基本

1. 好きな場所にライブラリ置く
2. ライブラリを登録
3. 使う

### ライブラリの登録について

付属の sym-lib-table, fp-lib-table には公式のgithubライブラリとこのライブラリを登録済み  
初期画面の [設定] -> [パスを編集]でそれぞれ

| 環境変数 | パス位置 |
----|----
| KICAD_SYMBOL | 公式 symbol パス |
| KISYSMOD |  公式 footprint パス |
| KUTKICAD |  KUTKiCad のリポジトリパス |

を登録し、この2つのファイルをプロジェクトフォルダに入れることで、  
プロジェクトファイルとして利用可能

***※注意***  
KISYSMODは初期はKiCad本体にあるローカルライブラリが登録されている  
作者はgithubでええやんと思っているので、グローバルを作らない前提で書き換えている  
もしそちらも利用したいなら適宜table内の環境変数書き換えてね

楽しい kicad life を！

P.S.
バトルキメランテス（ https://github.com/RobotClubKut/kicad-library ）は死んだ！  
昔のほう（ https://github.com/KUT-KiCad ）にあとでmarge予定