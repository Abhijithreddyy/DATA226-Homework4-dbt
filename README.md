# DATA226 Homework 4 - dbt

This project demonstrates a dbt transformation pipeline using Snowflake.

## Project Components

- Snowflake source tables in `DEMO_DB.RAW`
- Ephemeral transformation models
- Analytics table in `DEMO_DB.ANALYTICS`
- Snapshot table in `DEMO_DB.SNAPSHOT`
- Data quality tests for `sessionId`

## Project Structure

```text
dbt_project.yml
models/
├── sources.yml
├── schema.yml
├── transform/
│   ├── user_session_channel.sql
│   └── session_timestamp.sql
└── analytics/
    └── session_summary.sql
snapshots/
└── snapshot_session_summary.sql
