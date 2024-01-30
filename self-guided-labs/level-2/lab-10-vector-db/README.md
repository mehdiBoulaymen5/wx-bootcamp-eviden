## Milvius - Vector DB

### Install Milvus Lite
Milvus Lite is available on PyPI, you can install it via pip
python3 -m pip install milvus

Or, install it with PyMilvus as follows:
python3 -m pip install milvus[client]


### Install Milvius Standalone
For the users using MacOS 10.14 or later, set the Docker virtual machine (VM) to use a minimum of 2 virtual CPUs (vCPUs) and 8 GB of initial memory. Otherwise, installation might fail.

1. Download milvus-standalone-docker-compose.yml and save it as docker-compose.yml manually, or with the following command.
   wget https://github.com/milvus-io/milvus/releases/download/v2.3.1/milvus-standalone-docker-compose.yml -O docker-compose.yml
2. In the same directory as the docker-compose.yml file, start up Milvus by running:
   sudo docker compose up -d
3. Check the running containers:
   sudo docker compose ps
4. Verify which local port the Milvus server is listening on. Replace the container name with your own.
   docker port milvus-standalone 19530/tcp

### Use Milvius Standalone via TechZone
- https://techzone.ibm.com/collection/milvus-vector-database 


### Use provided examples from this repository
