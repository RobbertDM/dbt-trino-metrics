# dbt-trino-metrics
## Installation
In your `packages.yml`:
```
packages:
  - git: "https://github.com/robbertDM/dbt-trino-metrics"
    revision: 0.1.1
```

In your `dbt_project.yml`:
```
dispatch:
  - macro_namespace: metrics
    search_order: ['dbt_trino_metrics', 'metrics']
```

Then, run `dbt deps`. You should be good to go.
