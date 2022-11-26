CONFIG FOR NGINX

Each application cluster requires a different port, so we need a server configuration for each cluster, 
proper example has been provided in nginx folder

HOW TO RESTART EVERYTHING (ONLY WHEN NECESSARY)

RUN THESE COMMANDS AT ~/Monitoring folder

docker-compose down

docker-compose up -d

HOW TO RESTART SPECIFIC SERVICES

RUN THESE COMMANDS AT ~/Monitoring folder

docker ps

docker stop <old-process-id>

docker rm <old-process-id>

docker volume prune

docker-compose up -d --build