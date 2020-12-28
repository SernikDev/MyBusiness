# Electron-Forge React Boilerplate

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

The package includes a development environment for creating and building applications using Electron and React.

## Package can be run on:

- [x] linux
- [ ] windows (not tested)
- [ ] mac (not tested)

## Projects can be build for:

- [x] linux
- [x] windows
- [ ] mac

## Requirments

Docker version at least `19.03.8`

Docker Compose at least `1.25.0`

## Shell scripts permission

If you are receiving errors like `install.sh` command not found, You need to set executable permission to those files.

```
sudo chmod +x install.sh
sudo chmod +x run.sh
```

## .env

`USER_NAME` [required] - your user name account

`USER_ID` [required] - your user uid (you can check this in console with `echo $UID`)

`NODE_VERSION` [optional] - release node version

`CONTAINER_NAME` [optional] - docker container name

`APP_FOLDER_NAME` [optional] - if you want to change default `app` folder name, you might need to set this env

## Installation process

1. Create Your own repo by using this template feature on github or manually by downloading repo.
1. Create .env file using .env.example.
1. Inside project root directory run `sudo ./install.sh` and thats it.

## Commands

There is a script `run.sh` for start application container or make builds.

Available options:

`start` - starting docker container and run application

`stop` - stopping docker container

`build-linux` - building application for deb and rpm

`build-win` - building application for windows

## Example command usage

```
sudo ./run.sh start
```
