# Use a Docker Container to execute Jekyll

## Prerequisites

1. Docker has to be installed on your machine

## Step 1: Find an appropriate Docker Image

Docker is a system for running appliances including underlying operaing system in a closed container that will not interfere with your local system. Docker makes it possible to run completely preconfigured (and thus controlled) environments and basically any operation system.
So called Docker Images, i.e. definitions of virtual containers, are prebuilt containers and published through a docker registry, such as [Docker Hub](https://registry.hub.docker.com/).

A user submitted Docker Image for github pages is e.g. [starefossen/github-pages](https://registry.hub.docker.com/r/starefossen/github-pages).

## Step 2: Make sure Docker is runing on your machine

## Step 3: Build and run the MEI Website inside a Docker Container 

In order to build and run the MEI Website in a docker container follow the below steps. Please be aware that these steps are illustrated for Unix-based operating systems, e.g. macOS or Linux.

1. Switch to your local clone of the MEI Website

   ```bash
   cd PATH/TO/music-encoding.github.io
   ```

2. Execute Docker Image

   ```bash
   docker run --rm -it \
   --name meiWebsite \
   -p "4000:4000" \
   -v `pwd`:/usr/src/app \
   starefossen/github-pages
   ```
