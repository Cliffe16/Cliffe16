# Hi, I'm Cliffe Oluoch

**Data Engineer & Analytics Engineer** building resilient, production-ready ETL/ELT pipelines, real-time streaming architectures, and scalable analytical data stores.

* **Reach me**: [LinkedIn](https://www.linkedin.com/in/cliffeoluoch) • [oluochcliffe13@gmail.com](mailto:oluochcliffe13@gmail.com)

### Technical Stack

* **Languages & Frameworks**: Python, SQL (PostgreSQL, BigQuery, MySQL, T-SQL), KQL (Kusto), PySpark, FastAPI, Django, Bash
* **Streaming & Change Data Capture**: Apache Kafka, Debezium (PostgreSQL WAL CDC), Apache Spark Structured Streaming, Azure EventHub, Microsoft Fabric Eventstream
* **Orchestration & Transformation**: Apache Airflow, Astronomer Cosmos, dbt Core, MetricFlow, Fabric Data Factory, Celery, Redis
* **Cloud, Lakehouse & Warehousing**: Google Cloud Platform (BigQuery, GCS), Microsoft Fabric (OneLake, Eventhouse/KQL DB, Data Activator), Apache Cassandra, PostgreSQL, Neon
* **Data Modeling & Quality**: Kimball Star Schema, Medallion Architecture (Bronze/Silver/Gold), SCD Type 2, dbt tests, Dead-Letter Queue (DLQ) routing, GitHub Actions CI
* **Data Extraction & DevOps**: BeautifulSoup4, Headless Selenium WebDriver, Pandas, Requests, uv, Docker, Grafana

### Featured Engineering Projects

#### [NBA Analytics Pipeline](https://github.com/Cliffe16/NBA-Analytics-Pipeline)

> Production-grade ELT pipeline extracting daily NBA game and player performance stats, staging raw Parquet files in Google Cloud Storage, and modeling analytics in BigQuery using dbt Core and Apache Airflow.

* **Orchestration & Transformation**: Astronomer Cosmos rendering dbt models as native Airflow task groups inside Docker containers, with exponential backoff and rate-limit handling.
* **Dimensional Modeling & Semantic Layer**: Kimball Star Schema, SCD Type 2 paired with MetricFlow semantic metrics.
* **Data Quality & Serving**: Automated dbt schema and custom SQL data quality assertions, backed by a FastAPI service querying BigQuery marts.

#### [Hybrid Binance Crypto Market Pipeline](https://github.com/Cliffe16/Hybrid-Binance-Crypto-Market-Pipeline)

> Enterprise-grade Lambda architecture pipeline bridging batch extraction and real-time streaming across 3,700+ Binance cryptocurrency pairs (115,000+ data points) with zero data loss.

* **CDC & Event Streaming**: Airflow DAGs ingest order books, candlesticks, and tickers into PostgreSQL; Debezium captures row-level Write-Ahead Log (WAL) changes and streams events into Apache Kafka.
* **Distributed Stream Processing**: PySpark Structured Streaming consumes Kafka topics in 30-second micro-batches to flatten nested JSON payloads and compute 1-minute windowed spread and volume aggregations.
* **High-Throughput Serving & Observability**: Writes aggregated metrics to Apache Cassandra and exposes REST endpoints via FastAPI feeding a live Grafana dashboard, orchestrated via Docker Compose with tuned JVM heap limits.

#### [Agricultural Commodity Engine on Microsoft Fabric](https://github.com/Cliffe16/fabric-agri-commodity-engine-pipelines)

> Hybrid real-time and batch data platform on Microsoft Fabric delivering liquidity and volatility insights by combining historical FAOSTAT crop yield datasets with live Yahoo Finance commodity streams.

* **Real-Time Streaming & Alerting**: Offloads continuous Python polling to scheduled GitHub Actions to optimize Fabric F-SKU compute capacity, streaming via Azure EventHub SDK into Fabric Eventstream, a KQL Eventhouse (5-minute tumbling windows), and Data Activator (Reflex) for price volatility alerts.
* **Medallion Lakehouse & DLQ Resilience**: Fabric Data Factory and PySpark notebooks transform raw FAOSTAT API payloads across Bronze, Silver, and Gold Delta Parquet tables in OneLake, featuring threshold-based Dead-Letter Queue routing that quarantines anomalies under 10% and halts execution on critical spikes.
* **Automated QA & Governance**: Enforces pre-promotion PySpark validation alongside Entra ID pass-through authentication and T-SQL Row-Level Security (RLS).

### GitHub Activity

[https://github-stats-extended.vercel.app/api?username=Cliffe16&show_icons=true&theme=radical&hide_border=true]
[https://github-stats-extended.vercel.app/api/top-langs/?username=Cliffe16&layout=compact&theme=radical&hide_border=true]
