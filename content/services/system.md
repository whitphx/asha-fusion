---
Title: System
Img: asha-system.png
Category: Services
weight: 10
id: system
Draft: false
---

現バージョンのASHA fusionはWebベースのアプリケーションです．
サーバ機ではASHA fusionを各クライアントに配信するWebサーバと，データを保持するデータベースサーバが動作します．

データベースは[CouchDB](http://couchdb.apache.org/)およびCouchDBのJavaScriptクローンである[PouchDB](https://pouchdb.com/)を採用しています．
CouchDBはMaster-Master型のレプリケーションシステムを提供し，各デバイスのCouchDB間でシームレスにデータを同期します．
また，PouchDBはCouchDBのプロキシとして動作でき，ローカル/リモートを意識せず透過的にデータベースにアクセスできます．

CouchDBはスキーマレスDBなので，項目の追加・削除やデータ構造の変更が容易です．
使用シーンによって収集するデータを柔軟に変えることができます．
