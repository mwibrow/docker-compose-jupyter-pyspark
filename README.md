# docker-compose jupyter/pyspark-notebook

Simple example of using docker-compose to set up the
[jupyter/pyspark-notebook](https://github.com/jupyter/docker-stacks/tree/master/pyspark-notebook) image with a local volume.

This enables files to be exchanged between the container
and the host machine.

## Get started

Use the following command at the root of the project:

```
docker-compose up -d --build pyspark-notebook
```

This will pull everything, build and start the container.

To get the logs (in order to see the Jupyter access token) use:

```
docker-compose logs -f --tail 100 pyspark-notebook
```

Currently the default user directory of the container
is mapped to `./docker/volumes/pyspark-notebook`.
