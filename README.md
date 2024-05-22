# Task: *Create a data processing pipeline to transform and store log data.*

**Specifications**:

- **Language**: Python
- **Framework**: Use any combination of Pandas, NumPy, and Flask.
- **Tools**: Docker for containerization.

**Pipeline Overview**:

1. **Data Ingestion**: Ingest log data from a provided source file (CSV format).
2. **Data Transformation**: Clean and transform the data (e.g., parse timestamps, filter out specific log levels).
3. **Data Storage**: Store the transformed data in a SQLite database (or fake in memory storage).
4. **API Endpoints**:
    - **`GET /logs`**: Retrieve all logs.
    - **`GET /logs/:level`**: Retrieve logs of a specific level.
    - **`POST /logs/refresh`**: Trigger the ingestion and transformation process manually.

## Start and Reload App:
```
uvicorn main:app --reload
```

## Dependencies
Refer to the documentation for how to handle dependecies in fastapi.
https://fastapi.tiangolo.com/tutorial/dependencies/