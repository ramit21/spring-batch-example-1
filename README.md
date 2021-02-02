# Spring Boot with Spring Batch Example 1
## Load CSV to DB
- `http://localhost:8081/load` - Trigger point for Spring Batch
- `http://localhost:8081/h2-console` - H2 Console for querying the in-memory tables which contain transformed data as written by the batch job.

## H2 Config
- `testdb` - Database.
- `sa` - User
- `password` - Password.

## Theory

See Theory screenshot. Each job can have 1 or more steps (use flow() and next() functions in case of multiple steps). Each step can have Item-Reader/Processor/Writer. See SpringBatchConfig.java.

When creating project from Spring.io, select 'batch' as a required dependency. 

