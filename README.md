## mongodb replicaset compose

This guide will walk you through setting up a MongoDB Replicaset with docker compose

### Prerequisites

- [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed

### Getting started

1. Clone the repo
2. Navigate to the project directory
3. Create the MongoDB Replicaset using the command:

```bash
docker-compose up -d
```

4. Then when the containers are up, you can connect to the mongodb replicaset by typing:

```bash
docker exec -it mongo1 mongosh
```

5. Finally, you can check the status of the replicaset by typing:

```bash
rs.status()
```

You should be able to see the 3 members of the replicaset with one PRIMARY  and two SECONDARY 
