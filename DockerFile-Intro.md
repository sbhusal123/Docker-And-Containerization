# Dockerfile 
- Textfile with instruction to build images.
- Automation of Docker images.
- ``docker build .`` to build image from Dockerfile.
- [List of available commands](https://kapeli.com/cheat_sheets/Dockerfile.docset/Contents/Resources/Documents/index). 
- [Dockerfile Best-Practices Official docs](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#add-or-copy)


## Creating  custom python images with dockerfile for django setup:

#### 1. Create a requirements.py and add all the python dependencies on it.
```text
Django>=2.0,<3.0
psycopg2>=2.7,<3.0
```
#### 2. Create a Dockerfile.
```Dockerfile
FROM python:3
ENV PYTHONUNBUFFERED 1
RUN mkdir /app
WORKDIR /app
COPY requirements.txt /app
RUN pip install -r requirements.txt
```
**Description**
- ``FROM python:3``: grabs the python:3 image from the DockerHub(public registry).
- ``ENV PYTHONUNBUFFERED 1``: creates a environment variable **PYTHONUNBUFFERED** and sets it to **1**.
- ``RUN mkdir /app``: Creates a directory app.
- ``WORKDIR /app``: sets working directory to **app** inside the image.
- ``COPY requirements.txt /app``: copies the textfile  requirements.txt(root folder) into app(image folder) directory from. 
- ``RUN pip install -r requirements.txt``: Installs the packages listed in the requirements.txt file. 

#### 3. Build the image from the Dockerfile.
- ``docker build -t djangoimage:1 .``
    - ``-t djangoimage:<tag>``: names the image thus build as djangoimage with tag 1





