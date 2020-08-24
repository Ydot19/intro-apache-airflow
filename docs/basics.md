# Airflow Introduction

Airflow is a platform to programmatically
- Author
- Schedule
- Monitor 

works or data pipelines

## Basic Concepts

### Workflow

- A sequence of tasks
- Started on a schedule or triggered by an event
- Frequently used to handle big data processing pipelines


### Problems It Helps Solve

- Failures
    - Allows you to retry upon failure
    - Allows you to specify how many times to retry a job/task
- Monitoring
    - Success or failure status at each stage
    - How long does the process/stage run
- Dependencies
    - Data dependencies; upstream data is missing
    - Execution dependencies: upstream data is missing
    - Execution dependencies: job 2 runs after job 1 is finished
- Scalability
    - There is no centralized scheduler between different cron machines
- Deployment
    - Deploy new changes constantly
- Process Historic Data
    - Backfill/rerun historical data

### Benefits of Airflow

- Can handle upstream/downstream dependencies gracefully
    - Upstream missing tables
- Easy to re-process historical jobs by date, or re-run for specific intervals
- Jobs can pass parameters to other jobs downstream
- Handle errors and failures gracefully
- Ease of deployment of workflow changes (continuous integration)
- Integrations with a lot of infrastructure
    - Hive
    - Spark
    - Presto
    - Druid
    - AWS
    - GCP
    etc.
- Data sensors to trigger a DAG when data arrives
- Job testing through airflow itself
- Accessibility of log files and other meta-data through the web GUI
- Implement trigger rules for tasks
- Monitoring all jobs status in real time + Email alerts