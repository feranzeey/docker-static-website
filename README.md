# Docker Static Website

This project demonstrates how to containerize a simple HTML website using Docker and Nginx.

## Project Goal

Learn how Docker can package and run a web application in an isolated environment.

## Files

* index.html
* Dockerfile

## Dockerfile

FROM nginx:latest
COPY index.html /usr/share/nginx/html/index.html

## Build the Docker Image

docker build -t docker-website .
## Run the Container

docker run -p 8080:80 docker-website

Open browser:

http://localhost:8080

## What You Learn

* Docker image creation
* Container execution
* Serving static websites using Nginx
