# Titanic_Kaggle_competition
This is my repository for my participation in to the Titanic Kaggle competition

# Video Guide

[![Video Guide](https://img.youtube.com/vi/8yZMXCaFshs/1.jpg)](https://www.youtube.com/watch?v=8yZMXCaFshs)

# Project containter - Docker

## Install
You can use `Docker` to easily install all the needed packages and libraries:

### Build Docker

- **CPU:**
```bash
$ docker build -t casjar_titanic --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) -f docker/Dockerfile .
```
### Run Docker

- **CPU:**
```bash
$ docker run --rm --net host -it \
    -v $(pwd):/home/app/src \
    --workdir /home/app/src \
    casjar_titanic \
    bash
```
