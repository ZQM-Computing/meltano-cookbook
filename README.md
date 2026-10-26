# Meltano Cookbook

<!-- ZQM-START -->
<!-- markdownlint-disable MD033 -->
<p align="center">
  <strong>ZQM Computing — Geospatial Engineering & Scientific Computing</strong><br>
  <a href="https://github.com/ZQM-Computing">ZQM Computing</a>
</p>
<!-- markdownlint-enable MD033 -->
<!-- ZQM-END -->

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

A **Meltano cookbook** — Singer-based ELT pipelines as code. Planned in the Docker set; deployment pending on the fleet. Patterns are planned from the design, not yet from verified runs. It is intended for Data engineers who define ELT pipelines in versioned configuration. Validate each pattern against your own data, software versions, and operating environment before adopting it.

## Repository role and status

**Status:** Active, public — seeding. Pattern passes land in follow-up work from fleet-verified setups; the tables below list what is planned, not what is already written.

**What this repository is:** Meltano patterns — see the table below.

**What it contributes:** Part of the ZQM Computing geospatial portfolio. The umbrella index for the series is [geospatial-cookbooks](https://github.com/ZQM-Computing/geospatial-cookbooks).

**Standing:** This repository is maintained independently. Automated checks cover only the paths and environments configured in its workflows; they do not establish production readiness or operational certification.

## Who this is for

Data engineers who define ELT pipelines in versioned configuration.

## Prerequisites

- Meltano via Docker or pip
- Postgres or DuckDB as a destination
- Source credentials, kept out of repos

## Patterns (planned)

| # | Example | What it will demonstrate |
|---|---------|--------------------------|
| 01 | `01-first-project` | A first Meltano project: taps, targets, and jobs |
| 02 | `02-postgres-target` | Loading into Postgres with a target plugin |
| 03 | `03-schedules` | Scheduled jobs and environments |
| 04 | `04-dbt-pairing` | Transforming loaded tables with dbt (see dbt-cookbook) |

## Repository layout

```text
meltano-cookbook/
├── examples/          # pattern passes, landing in follow-up work
├── README.md
└── LICENSE
```

## Roadmap

- First pattern pass: the first two table rows
- Second pass: the remaining rows, from fleet-verified setups

## Contributing

A contributing guide lands with the first pattern pass. Report security issues to <zqmcomputing@gmail.com> — please do not open a public issue for those.

## More from this series

- [dlt-cookbook](https://github.com/ZQM-Computing/dlt-cookbook) — ELT pipelines from Python into Postgres and DuckDB
- [airbyte-cookbook](https://github.com/ZQM-Computing/airbyte-cookbook) — Connector-based ELT into Postgres and DuckDB
- [dbt-cookbook](https://github.com/ZQM-Computing/dbt-cookbook) — SQL transformations, models, and tests on Postgres
