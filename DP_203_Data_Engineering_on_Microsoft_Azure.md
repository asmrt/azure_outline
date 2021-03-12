# DP-203：Data Engineering on Microsoft Azure (beta） Outline (Japanese)

- 原文
    - https://docs.microsoft.com/en-us/learn/certifications/exams/dp-203

## DP-203：Data Engineering on Microsoft Azure (beta）とは

```
Azureデータエンジニアは、分析ソリューション構築に適した構造で、統合?（integrate）、変換、統合?（consolidate）することで
さまざまな構造化および非構造化データシステムから構造化します。
試験DP-203の候補者：「Data Engineering on Microsoft Azure」では、SQL、Python、Scalaなどのデータ処理言語の
確固たる知識を持ち、並列処理やデータアーキテクチャパターンを理解している必要があります。
```

## 評価されるスキル

### データストレージの設計と実装(40-45%)

- データストレージ構造の設計
    - Azure データレイクソリューションの設計
    - ストレージとして推奨ファイル種類
    - 分析クエリのための推奨ファイル種類
    - 効率的なクエリ設計
    - データプルーニング（刈り込み）の設計
    - データ変換のレベルを表すフォルダ構造の設計
    - 流通戦略の設計
    - データ・アーカイブソリューションの設計

- パーティション戦略の設計
    - ファイルのパーティション戦略の設計
    - 分析ワークロードのためのパーティション戦略の設計
    - 効率と性能のためにパーティション戦略の設計
    - Azure Synapse Analyticsのパーティション戦略の設計
    - Azure Data Lake Storage Gen2でパーティショニングが必要な場合の識別

- サーバ層の設計
    - スタースキーマの設計
    - ディメンション表のゆるやかな設計
    - 次元階層の設計
    - 一時データのソリューションの設計
    - 増分ロードの設計
    - 分析のストレージ領域の設計
    - Azure Synapse AnalyticsとAzure Databricksでメタストアの設計
- 物理データストレージ構造の実装
    - 圧縮の実装
    - パーティショニングの実装
    - シャーディングの実装
    - Azure Synapse Analytics プールを使用して異なるテーブル ジオメトリの実装
    - データの冗長性の実装
    - 分散テーブルの実装
    - データアーカイブの実装

- 論理データ構造の実装
    - 一時的なデータソリューションの構築
    - ゆるやかなディメンション表の構築
    - 論理フォルダ構造の構築
    - 外部テーブル（external tables）の構築
    - 効率的なクエリとデータのプルーニングのためのファイルおよびフォルダ構造の実装

- サーバ層の実装
    - リレーショナルスタースキーマでのデータ提供
    - Purquetファイルでのデータ提供
    - メタデータの管理
    - 次元階層の実装
 
### データ処理の設計・開発（25～30%)

- データの読み込みと変換
    - Apache Sparkを使ってデータの変換
    - Transact-SQLを使ってデータの変換
    - Data Factoryを使ってデータの変換
    - Azure Synapse Pipelinesを使用してデータを変換する
    - Stream Analyticsを使ってデータの変換
    - データのクリーンアップ
    - データの分割
    - JSONデータの細断
    - データ符号化 / 復号化
    - 変換時のエラー処理の設定
    - 値の正規化と非正規化
    - Scalaでデータの変換
    - データの探索分析の実施

- バッチ処理ソリューションの設計・開発
    - Data Factory、Data Lake、Spark、Azure Synapseパイプライン、PolyBase, Azure Databricksを利用したバッチ処理ソリューションの開発 シナプスパイプライン、PolyBase、Azureデータバンク
    - データパイプラインの作成
    - 増分データロードの設計と実装
    - じわじわと変化するディメンション表の設計・開発
    - セキュリティとコンプライアンスの要件への対応
    - リソースのスケーリング
    - バッチサイズの設定
    - データパイプラインのテスト設計・作成
    - Jupter/IPythonノートブックのデータパイプライン統合
    - 重複データハンドリング
    - 欠損データハンドリング
    - 遅延データハンドリング
    - データのUPSERT
    - 元の状態に戻す
    - 例外処理の設計と設定
    - バッチ保有設定
    - バッチ処理ソリューション設計
    - Spark UIを使ってSparkジョブをデバッグ

- ストリーム処理ソリューションの設計・開発
    - Stream Analytics、Azure Databricks,Azure Event Hubsを利用したストリーム処理ソリューションの開発
    - Sparkの構造化ストリーミングを利用したデータ処理
    - パフォーマンスと機能リグレッション（デグレ？）の監視
    - Window関数の設計と作成
    - Schema Drift（ソースデータの構造の変更）の操作
    - 時系列データの処理
    - パーティションをまたぐ（across）処理
    - 処理中のチェックポイント/Watermarkingの設定
    - リソースのスケール
    - データパイプラインのテスト設計・作成
    - 分析またはトランザクションのためのパイプラインの最適化
    - 割り込みの操作
    - 例外処理の設計と設定
    - データのUPSERT
    - アーカイブされたストリームデータの再生
    - ストリーム処理ソリューションの設計

- バッチとパイプラインの管理
    - trigger batches
    - 失敗したバッチロードの操作
    - バッチロードの検証
    - DataFactory/Synapse Pipelineでデータ パイプラインの管理
    - DataFactory/Synapse Pipelineでデータ パイプラインのスケジュール
    - パイプライン・アーティファクトのためのバージョン管理の実装
    - パイプラインでSparkジョブの管理

### Design and Implement Data Security：データセキュリティの設計・実装（10～15%）
- データポリシーと標準化のためのセキュリティ設計
    - データの暗号化の設計
    - データ監査戦略（auditing strategy）の設計
    - データマスキング戦略を立てる
    - データプライバシーの設計
    - データ保持ポリシーの策定
    - ビジネス要件に基づいてデータをパージの設計
    - Data Lake Storage Gen2のためのAzureロールベースアクセス制御(Azure RBAC)とPOSIXライクなアクセス制御リスト(ACL)の設計
    - 行レベルおよび列レベルのセキュリティの設計

- データセキュリティの実装
    - データマスキングの実装
    - 安静時と移動時のデータの暗号化
    - 行レベル（row-level）および列レベル（column-level）のセキュリティの実装
    - Azure RBACの実装
    - Data Lake Storage Gen2 の POSIX ライクな ACL の実装
    - データ保持ポリシーの実施
    - データ監査戦略（data auditing strategy）の実装
    - 異なるデータ・プラットフォーム・テクノロジーにまたがる identities、Key 、Secretの管理
    - 安全なエンドポイントを実装する
    - Azure Databricksでのリソーストークンの実装
    - 機密情報（sensitive information）を含むDataFrameを読み込む
    - 暗号化されたデータをテーブルやParquetファイルに書き込む
    - 機密情報（sensitive information）の管理


### データストレージとデータ処理の監視と最適化(10-15%)
- データストレージとデータ処理の監視
    - Azure Monitorを使ったロギングの実装
    - 監視サービスの構成
    - データの動きのパフォーマンスの測定
    - システム全体のデータに関する統計の監視、更新
    - データパイプラインの性能の監視
    - query performanceの測定
    - cluster performanceの監視
    - custom logging optionsの理解
    - パイプラインテストのスケジュールと監視
    - Azure Monitorのメトリクスとログ（ metrics and logs）の解釈
    - Sparkの有向非周期グラフ(DAG（directed acyclic graph）)の解釈


- データストレージとデータ処理の最適化とトラブルシューティング
    - compact small files
    - ユーザー定義関数(UDF ：user-defined function)の書き換え
    - データのスキュー（skew , 偏り？）の扱い
    - shuffle partitions の調整
    - パイプラインでのシャッフル箇所の探索
    - 資源管理の最適化
    - データベース索引を使用したクエリの調整
    - キャッシュを使ってクエリの調整
    - 分析またはトランザクションのためのパイプラインの最適化
    - 記述的VS分析的なワークロードのためのパイプラインの最適化
    - 失敗したSparkジョブのトラブルシューティング
    - 失敗したパイプラインのトラブルシューティングの実行
