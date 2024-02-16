# Docker compose template for Elasticsearch and Kibana for small to medium servers
Template for Docker Compose to Elasticsearch and Kibana containerization suitable for small to medium servers.

## Customizable options
- Elasticsearch version
- Kibana version
- Elasticsearch data path
- Elasticsearch memory settings
- Kibana memory settings
- Elasticsearch plugins
- Kibana plugins
- Port mapping

## Mounting a volume for Elasticsearch data
In this docker-compose template, `/usr/share/elasticsearch_docker_volumes` is being used for mounting a volume for Elasticsearch data. You can change this to any directory you want. Either you opt to this path or not, you need to create the directory and change its permission for user `elasticsearch` before running the docker-compose command.
    
```bash
sudo mkdir -p /usr/share/elasticsearch_docker_volumes
sudo chown -R 1000:1000 /usr/share/elasticsearch_docker_volumes
```
