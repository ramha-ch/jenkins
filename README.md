Simple HTML Project with Docker and Nginx
This repository contains a simple HTML project deployed using Docker with NGINX as the web server.

Project Overview
A basic HTML website hosted on NGINX for a seamless and responsive user experience.
Docker is used for containerization to simplify the deployment process.
Prerequisites
Docker should be installed on your system.
Basic knowledge of web development and HTML.
Project Structure

Docker Setup
dockerfile
Copy code
FROM nginx
COPY . /usr/share/nginx/html/

The Dockerfile uses NGINX as the base image and copies the contents of the current directory to the default NGINX web root (/usr/share/nginx/html/).
Building and Running the Docker Image
Build the Docker image:

bash
Copy code
docker build -t simple-html-nginx .
Run the Docker container:

bash
Copy code
docker run -d -p 80:80 simple-html-nginx
Access your website:

Open your web browser and navigate to http://localhost.
