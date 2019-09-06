# Specify 7 in Docker

Dockerized version of [Specify 7](https://github.com/specify/specify7).

Specify 7 is build upon Specify 6, so you need a running instance of Specify 6.

## Installation

- Clone this repository.
  ```
    git clone https://github.com/rbgvictoria/specify7-docker.git
  ```

- Copy your Specify 6 client into the `specify7/specify6_thick_client` directory

- Rename `example.local_specify_settings.py` in `specify7/specify7_config` to `local_specify_settings.py`

- Add your database connection details in `local_specify_settings.py`

- Build the Docker image and start the container
  ```
    cd specify7-docker
    docker-compose up -d
  ```
  Your Specify 7 instance should now be available at `http://localhost:<port>`. I use port number 65001; you can change the port in the `docker-compose.yml` file.



