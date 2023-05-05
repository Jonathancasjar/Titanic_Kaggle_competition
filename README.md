# Titanic_Kaggle_competition
This is my repository for my participation in to the Titanic Kaggle competition

#Video Guide

<video width="320" height="240" controls>
  <source src="https://www.youtube.com/watch?v=8yZMXCaFshs" type="video/mp4">
</video>


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
