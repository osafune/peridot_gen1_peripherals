PERIDOTペリフェラル集
=====================

PERIDOTコンフィグレーションで使用している標準ペリフェラル集です。


対象となるツール
================

PERIDOTボードおよびQsys

使い方
------

- ip以下のフォルダをcloneして、プロジェクトのローカルに保存するか、保存場所にライブラリパスを通します。
- Qsysでコンポーンネントをaddして適宜操作します。

ペリフェラルのレジスタについてはdoc以下のpdfを参照してください。


ペリフェラルの概要
==================

PERIDOT Avalon Bridge
---------------------

ホストからQsys内部へアクセスするブリッジを提供します。  
Chromeアプリでは[Canarium.js](https://github.com/osafune/peridot/tree/master/sample_apps)を利用することでJavaScriptからQsys内部のAvalon-MMスレーブペリフェラルにアクセスすることができます。  


PERIDOT SWI
-----------

PRIDOTプロセッサ(NiosII)とホストとの排他制御や、ホストからの通知、ブートシーケンス制御の機能を提供します。  
PERIDOT標準システムではQsys SystemIDペリフェラルと合わせて、PERIDOTコンフィグレーションのシステム情報ブロックを構築します。  


PERIDOT PFC
-----------

PERIDOTのピンマトリックスセレクタおよび制御用のインターフェースを提供します。  


PERIDOT I2C
-----------

PERIDOT標準ペリフェラルで使用されるコンパクトなI2Cホストペリフェラルです。  


PERIDOT SPI
-----------

PERIDOT標準ペリフェラルで使用されるコンパクトなSPIホストペリフェラルです。  


PERIDOT SERVO
-------------

PERIDOT標準ペリフェラルで使用されるRCサーボ用コントローラです。  
周期20ms、パルス幅0.5～2.5msのPWM波形を256段階で出力します。また、設定値をアナログ出力するための1bitΔΣ変調出力を持ちます。  


ライセンス
=========

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
