# ELT Pipeline with dbt, Snowflake, and Airflow

This project demonstrates how to build an ELT pipeline using industry-standard tools: **dbt**, **Snowflake**, and **Airflow**. The goal is to show a practical, step-by-step approach to modern data engineering, including data modeling, orchestration, and deployment.

## Steps Covered

- Set up dbt with Snowflake
- Configure `dbt_project.yml` and install packages
- Create source and staging tables
- Build transformed models (fact tables, data marts)
- Write macro functions for reusable logic
- Implement generic and singular tests for data quality
- Deploy models using Airflow for orchestration
- Apply Snowflake RBAC concepts for secure access

## Project Structure

- **dags/**: Airflow DAGs for pipeline orchestration
- **Dockerfile**: Astro Runtime Docker image for Airflow
- **include/**: Extra files (optional)
- **packages.txt**: OS-level dependencies (optional)
- **requirements.txt**: Python dependencies (optional)
- **plugins/**: Custom Airflow plugins (optional)
- **airflow_settings.yaml**: Airflow Connections, Variables, and Pools

## Getting Started

To run Airflow locally:

```sh
astro dev start
```

- Access Airflow UI: [http://localhost:8080/](http://localhost:8080/)
- Postgres DB: `localhost:5432/postgres` (user: `postgres`, password: `postgres`)

If you encounter port issues, refer to the [troubleshooting guide](https://www.astronomer.io/docs/astro/cli/troubleshoot-locally#ports-are-not-available-for-my-local-airflow-webserver).

## Deployment

To deploy your code to Astronomer, follow the [deployment documentation](https://www.astronomer.io/docs/astro/deploy-code/).

## Feedback

Have suggestions or want to see other Data Engineering topics? Drop your ideas in the comments!

---