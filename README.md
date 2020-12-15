# velopark-db
Docker configuration to setup Velopark's platform database.

## Configure it

1. First download the database dump (`mongodb-dump` folder) that contains all the currently existing Velopark DB data from [here](https://cloud.ilabt.imec.be/index.php/s/MNLtEc5jMXx3C9f).
2. Configure the `volume` path to the persistent folder that will hold the database data by replacing `/path/to/persistent/folder` for your own path [here](https://github.com/julianrojas87/velopark-db/blob/43845585a3f485b31f92b7bf36143f8dbb06fa1e/docker-compose.yml#L9).
3. Configure the `volume` path of the database dump that will be restored by replacing `/path/to/mongodb-dump` for the folder downloaded in step 1 [here](https://github.com/julianrojas87/velopark-db/blob/43845585a3f485b31f92b7bf36143f8dbb06fa1e/docker-compose.yml#L15).

## Run it

Execute `docker-compose up`.

