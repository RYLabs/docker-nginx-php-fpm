# Docker base image for PHP applications using Nginx+FPM

This serves as a base image for R&Y Lab's base Docker image for [docker-craftcms](https://github.com/RYLabs/docker-craftcms).

This image combines the official Docker PHP FPM image with instructions for the official Nginx image and runs both using Supervisord. Composer is also provided for convenience. This setup works around an issue with getting file permissions right when working with container volumes and the PHP process needing to write to the project direct (like CraftCMS).
