# Great Expectations dbt + Airflow Pipeline Tutorial

The purpose of this example is to show how Airflow can orchestrate a data quality pipeline using Great_expectations.



## This tutorial directory contains three Airflow DAGs of this data pipeline:
* `airflow/ge_tutorials_dag_without_great_expectations.py`
* `airflow/ge_tutorials_dag_with_great_expectations.py`
* Data quality validation DAGs `airflow/ge_airflow_quick_start.py`


## Setup

### Setup with Docker

```
git clone
cd ge_tutorials/ge_dbt_airflow_tutorial
# you can run this command every time you need to start:
docker-compose up
```

Once these steps are completed, you can access Airflow at http://localhost:8080/admin/.

To run the DAG, you first need to turn it on, then manually trigger it. You can do so through the UI:

Once the DAG has run successfully, you'll be able to access the Great Expectations Data Docs at the following URL: http://localhost:8081

Don’t forget to shut down the docker after you finish.

```
docker-compose down
```
