# docker-elk
Basic ELK stack in Docker

# NGinX - Version (Stable) -> 1.16.1

# Apache httpd - Version (Stable) -> 2.4.41

# outside the docker-compose run the nginx in dedicated mode use Docker CLI:
docker run -d -p 8080:80 --log-driver gelf --log-opt gelf-address=udp://localhost:12201 nginx:1.16.1

docker run -d -p 8080:80 --log-driver gelf --log-opt gelf-address=udp://localhost:12201 --name=nginx nginx:1.16.1

# ___ some links:
https://grafana.com/grafana/dashboards/2030
https://grafana.com/grafana/dashboards/6058