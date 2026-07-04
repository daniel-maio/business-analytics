# Geospatial SQL Analytics

A Geospatial Data Engineering pipeline that leverages DuckDB's native spatial and cloud extensions to query, filter, and merge building footprint datasets (Google, Microsoft, and OpenStreetMap).

## Data Source

https://source.coop/products

## Features

- Serverless Cloud Data Ingestion: Connects directly to `Source.coop` via DuckDB's HTTPFS and Spatial extensions, downloading partitioned GeoParquet metadata and building rows based on regional ISO partitioning.
- Spatial Intersection & Clipping: Loads regional boundary files (`.geojson`), maps coordinates into data tables (`area_of_interest`), and executes spatial clipping optimizations using `ST_Intersects` and `ST_Intersection` geometries.
- Deduplication Engine (Geo-Spatial Join): Combines layers using an intersection via SQL queries. It performs a selective `UNION ALL` that evaluates building overlap using Intersection over Union (IoU) ratios, discarding records where spatial intersection areas share an explicit ratio.

## Quickstart
```bash
pip install duckdb geopandas pyarrow lonboard requests
```

---