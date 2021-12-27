# Dockerfile-for-windowservice-and-python
## Structure
  1. windowsservice_dockerfile - Creates multilevel docker and moves python to ws directory based on the alias name
  2. docker-compose.yml - Creates image

## Execution
  >. docker build -f windowservice_dockerfile -t windowserviceimage .
  
  This commond builds image with tag windowserviceimage from windowservice_dockerfile to current directory
  
  >. docker-compose up -d
  
  This commond exceutes the docker-compose.yml where we linked windowserviceimage with container_name and makes the container up.
