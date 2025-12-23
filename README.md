# E-Commerce Analytics Microservice
Traditional SQL databases often experience performance bottlenecks when executing heavy analytical queries on large datasets. This project implements a dedicated analytics microservice using Elasticsearch to offload this processing. It exposes a REST API that delivers instant insights—such as daily revenue histograms, category performance rankings, and long-term growth trends—ensuring the primary transactional database remains unburdened.

# Use Cases
-> Ingest Sale: The system must be able to receive a new order/sale and index it into Elasticsearch.

-> Get Daily Revenue: The user can request total revenue grouped by day for a specific date range.

-> Get Trend Analysis: The user can request revenue grouped by month to visualize long-term growth trends (Date Histogram Aggregation).

-> Get Category Performance: The user can see which product categories are performing best (Bucket Aggregation).
