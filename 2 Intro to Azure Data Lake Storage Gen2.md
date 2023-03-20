# Intro to Azure Azure Data Lake Storage Gen2
https://learn.microsoft.com/en-us/training/modules/introduction-to-azure-data-lake-storage/1-introduction

- **data lake** contains unstructured data in its natural format
	- stored in files, not relational db
- store in data lake, then consume with big data tech (like Apache Spark)
- Azure Data Lake stores in Hadoop-friendly format
- data replication (disaster recovery) borrows from Azure Blob storage
- Azure Storage Explorer organizes similar to directory-and-file structure
- Azure Data Lake is a configurable option of Azure Storage V2. It's not really its own product

Azure Blob Storage uses flat namespace for non-analysis storage. Azure Data Lake uses hierarchical namespace, which is pre-organized and allows for faster analysis.

1. **Ingest** Identify data sources and find the best way to ingest them (stream, batch)
	Stream ingestion: Apache Kafka for HDInsight, Stream Analytics
	Batch ingestion: Azure Synapse Analytics, Azure Data Factory
2. **Store** Identify where data should be placed
3. **Prep & Train** Data preparation, plus model training and scoring for ML
	Azure Synapse Analytics, Azure Databricks, Azure HDInsight, Azure Machine Learning
4. **Model & Serve** Present the data to users (Power BI)

continue at https://learn.microsoft.com/en-us/training/modules/introduction-to-azure-data-lake-storage/6-use-cases