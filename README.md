# E-Commerce Analytics Microservice
Traditional SQL databases struggle with heavy analytical queries like 'rolling averages' on large datasets. This project implements a dedicated real-time analytics microservice layer using Elasticsearch. It exposes a REST API that allows frontend dashboards to retrieve complex metrics—like 7-day moving averages and day-over-day growth—instantly, without burdening the primary transactional database.

# Use Cases
-> Ingest Sale: The system must be able to receive a new order/sale and index it into Elasticsearch.

-> Get Daily Revenue: The user can request total revenue grouped by day for a specific date range.
-> Get Trend Analysis: The user can request the 7-day moving average to smooth out daily volatility ("Pipeline Aggregation" feature).
-> Get Category Performance: The user can see which product categories are performing best (Bucket Aggregation).
