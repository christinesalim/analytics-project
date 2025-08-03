#readme file for chapter 10


Run command to download the docker-compose.yaml file
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.10.0/docker-compose.yaml' 

Ran command to init docker env using docker-compose.yaml. I added overrides in docker-compose.override.yaml
docker compose up airflow-init 

Ran command to run container in detached mode using "-d" flag. Need to wait a few minutes, then go to ports tab in codespace and open UI using globe icon.
docker compose up -d

docker compose down      # Stop and remove running containers
docker compose up -d     # Recreate containers with the updated config

docker compose down --volumes --remove-orphans
