# Hello Docker

This is a simple "Hello World" Docker project in Python.

## Description

This project demonstrates how to create a Docker container for a Python application that prints "Hello World" to the console.

## Usage

1. *Build Docker Image*:
   First, build the Docker image using the provided Dockerfile:
   ```
   docker build -t hello-docker-python .
   ```
2.  Run Docker Container:

After building the image, you can run the Docker container to see the "Hello World" message:
```
docker run hello-docker-python
```
3. Push Docker Image to Docker Hub:

If you want to push the Docker image to Docker Hub, you need to tag the image with your Docker Hub username and repository name, and then push it:
```
docker tag hello-docker-python username/hello-docker-python:tag
docker push username/hello-docker-python:tag
```
Note: Replace username with your Docker Hub username and tag with the version or tag you want to assign to the image.

Contributing

Contributions are welcome! Please feel free to submit pull requests with improvements or additional features.

