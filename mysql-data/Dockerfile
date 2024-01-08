# Use an official MySQL image as the base image
FROM mysql:latest

# Environment variables for MySQL configuration
ENV MYSQL_ROOT_PASSWORD=root
ENV MYSQL_DATABASE=mydatabase
ENV MYSQL_USER=myuser
ENV MYSQL_PASSWORD=mypassword

# Copy MySQL schema initialization script to docker-entrypoint-initdb.d/
COPY ./init.sql /docker-entrypoint-initdb.d/

# Expose the port MySQL runs on (not mandatory in all setups)
EXPOSE 3306
