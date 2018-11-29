
# carddav2fb-docker

Provides an easy way to run carddav2fb (https://github.com/andig/carddav2fb) in a Docker container.

## Requirements

- Docker for Windows or Linux
- `Config.php` - Example -> https://github.com/andig/carddav2fb/blob/master/config.example.php

## How to build the image

1. Pull the repository
1. Switch into the directory
1. Download `config.example.php` from https://github.com/andig/carddav2fb/blob/master/config.example.php and enter your credentials. Rename it to `config.php`
1. Run the following command: `docker build -t carddav2fb-docker .`

## How to run the image

Run the following command: `docker run -it carddav2fb /bin/bash`

The import will begin automatically. When the import has finished,exit the container.

## Note

I tested the Docker file with the version available at that time (see commit of Docker file). If you have any importing issues, please check https://github.com/andig/carddav2fb as this repository just provide a simple way to run carddav2fb.