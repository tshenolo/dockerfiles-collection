# Dockerfiles Collection

This repository contains Dockerfiles for deploying web applications using different server-side languages and frameworks. Each directory in this repository represents a specific technology stack, and inside each directory, you will find a Dockerfile and any other necessary files for building and running a Docker container.

## Table of Contents

- [Stacks](#stacks)
  - [PHP (Apache)](#php-apache)
  - [Java (WAR)](#java-war)
  - [Node.js](#nodejs)
  - [Python (Flask)](#python-flask)
  - [Ruby (Ruby on Rails)](#ruby-ruby-on-rails)
  - [C# (ASP.NET Core)](#c-aspnet-core)
- [Usage](#usage)
  - [Building the Docker Image](#building-the-docker-image)
  - [Running the Docker Container](#running-the-docker-container)
- [Contributing](#contributing)
- [License](#license)

## Stacks

### PHP (Apache)

This Dockerfile is configured to run a PHP application with Apache.

- **Base Image:** `php:8.1-apache`
- **Exposed Port:** `80`

[View Dockerfile](php-apache/Dockerfile)

### Java (WAR)

This Dockerfile is set up to deploy a Java web application packaged as a WAR file using Tomcat.

- **Base Image:** `tomcat:10.1`
- **Exposed Port:** `8080`

[View Dockerfile](java-war/Dockerfile)

### Node.js

This Dockerfile is designed for a Node.js application.

- **Base Image:** `node:20`
- **Exposed Port:** `3000`

[View Dockerfile](nodejs/Dockerfile)

### Python (Flask)

This Dockerfile is configured for a Python web application using Flask.

- **Base Image:** `python:3.11`
- **Exposed Port:** `5000`

[View Dockerfile](python-flask/Dockerfile)

### Ruby (Ruby on Rails)

This Dockerfile is set up for a Ruby on Rails application.

- **Base Image:** `ruby:3.2`
- **Exposed Port:** `3000`

[View Dockerfile](ruby-rails/Dockerfile)

### C# (ASP.NET Core)

This Dockerfile is configured for a C# ASP.NET Core application.

- **Base Image:** `mcr.microsoft.com/dotnet/aspnet:7.0`
- **Exposed Port:** `80`

[View Dockerfile](csharp-aspnet/Dockerfile)

## Usage

### Building the Docker Image

To build a Docker image, navigate to the directory of the desired stack and run the following command:

```sh
docker build -t your-image-name .
```

### Running the Docker Container

To run the Docker container, use the following command:

```sh
docker run -p host-port:container-port your-image-name
```

Replace `host-port` and `container-port` with the appropriate port numbers as specified in each stack.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue if you have any suggestions or improvements.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

