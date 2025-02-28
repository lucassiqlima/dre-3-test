## Description
This project uses docker compose to start airflow components and run dags located into `dags/` path.
## Prerequisites
Before setting up the project, ensure you have the following installed:
Docker and Docker Compose: Required for running Airflow in a containerized environment.
## Setup
Clone the Repository:
``` bash
git clone git@github.com:lucassiqlima/dre-3-test.git
cd dre-3-test
```

Build and Start the Docker Containers:
``` bash
docker-compose up -d
```
Access the Airflow UI:
Open your browser and go to http://localhost:8080.

### Log in with the follow credentials:
**User**: airflow
**Password**: airflow
## Running the DAG
Enable the DAG:
- Go to the Airflow UI.
- Find the smooth_dag in the list of DAGs.
- Toggle the ON/OFF switch to enable it.
Trigger the DAG:
- Click the "Play" button to manually trigger the DAG.
- Alternatively, wait for the scheduled interval (if defined).
Monitor Progress:
- Use the Airflow UI to monitor task progress and logs.