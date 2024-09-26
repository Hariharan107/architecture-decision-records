# **Selecting a Database for Our Microservices Architecture**

- Status: proposed
- Date: 26 September 2024

## Context and Problem Statement

We need to choose an appropriate database system that can support our microservices architecture, ensuring scalability, performance, and data consistency across services.

## Considered Options

| Option | Pros | Cons |
| ------ | ---- | ---- |
| PostgreSQL | ACID compliant, strong consistency, rich feature set, excellent for complex queries and transactions | Vertical scaling can be challenging, may require more effort to set up for distributed systems. |
| MongoDB | Flexible schema, horizontal scalability, good performance for read-heavy workloads, native support for JSON-like documents. | Eventual consistency by default, less suitable for complex transactions, larger storage requirements. |
| Apache Cassandra | Excellent scalability and performance for write-heavy workloads, highly available, good for time-series data. | Limited support for complex queries, eventual consistency, steeper learning curve. |
| Amazon DynamoDB | Fully managed, auto-scaling, low latency, serverless-friendly, good for microservices. | Vendor lock-in, can be expensive for high-volume workloads, limited querying capabilities compared to SQL databases |

## Decision Outcome

The selected option is "**PostgreSQL**", based on the following key decision criteria: Scalability, performance, data consistency, ecosystem support, and compatibility with our existing tech stack..

## Links

* [Official PostgreSQL website](https://www.postgresql.org/)
* [AWS blog on microservices with PostgreSQL](https://aws.amazon.com/blogs/database/building-microservices-with-amazon-rds-and-amazon-aurora/)

## Appendix

Our team conducted performance tests with sample datasets and workloads representative of our expected usage. PostgreSQL showed the best balance of performance, consistency, and flexibility for our specific use cases.
