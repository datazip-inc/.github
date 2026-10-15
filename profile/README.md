<p align="center">
  <a href="https://olake.io"><img src="https://raw.githubusercontent.com/datazip-inc/olake-docs/master/static/img/logo/olake-blue-with-text.svg" alt="OLake" width="320"></a>
</p>

<p align="center">
  <b>Open-source replication of databases and Kafka into Apache Iceberg.</b><br>
  Built by <a href="https://datazip.io">Datazip</a>.
</p>

<p align="center">
  <a href="https://olake.io">Website</a> ·
  <a href="https://olake.io/docs">Docs</a> ·
  <a href="https://olake.io/blog">Blog</a> ·
  <a href="https://olake.io/slack">Slack</a> ·
  <a href="https://x.com/_olake">X</a>
</p>

---

## What we build

| Project | What it does |
|---|---|
| [**olake**](https://github.com/datazip-inc/olake) | CDC, full-refresh and incremental replication from PostgreSQL, MySQL, MongoDB, Oracle, SQL Server, DB2, Kafka and S3 into Apache Iceberg (or Parquet). Single Go binary, Apache-2.0. |
| [**olake-fusion**](https://github.com/datazip-inc/olake-fusion) | Iceberg table maintenance: compaction, snapshot expiry, orphan-file cleanup. |
| [**olake-ui**](https://github.com/datazip-inc/olake-ui) | Web UI and backend for configuring sources, destinations and sync jobs. |
| [**olake-helm**](https://github.com/datazip-inc/olake-helm) | Helm chart for running OLake on Kubernetes. |
| [**olake-docs**](https://github.com/datazip-inc/olake-docs) | Source for [olake.io](https://olake.io): docs, blog, customer stories. |
| [**workshops**](https://github.com/datazip-inc/workshops) | Hands-on workshops on Apache Iceberg and related tooling. |

## Why OLake

- **No Kafka Connect, Flink or Spark in the path.** OLake reads WAL / binlog / change streams and writes Iceberg directly.
- **Catalogs:** AWS Glue, REST, Hive, JDBC, Polaris, Nessie, Lakekeeper, Unity, Snowflake Open Catalog.
- **Operational:** parallel chunked backfills, schema evolution, checkpointed resumable state, exactly-once-style writes.
- **Runs anywhere:** CLI, Docker, Kubernetes (Helm). Optional web UI.

## Get started

```bash
docker run -it olakego/source-postgres:latest --help
```

Quickstart: https://olake.io/docs/getting-started

## Community

- Slack: https://olake.io/slack
- Issues and feature requests: https://github.com/datazip-inc/olake/issues
- Contributing guide: https://github.com/datazip-inc/olake/blob/master/CONTRIBUTING.md
- Benchmarks: https://olake.io/docs/benchmarks

Used in production by PhysicsWallah, AstroTalk, LendingKart, Cordial, Bitespeed and Xeno. Read the [customer stories](https://olake.io/customer-stories).
