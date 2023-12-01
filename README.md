# Docker Documentation

## Table of contents

-   [Installing Docker](#make-sure-docker-compose-is-installed)
-   [Test Docker](#command-to-test-docker-in-your-terminal)
-   [Docker Hub Login](#login-to-docker-hub)

## Make sure Docker Compose is installed

For Linux and Windows: [Docker Desktop or CLI Install](https://docs.docker.com/compose/install/)

## Command to test Docker in your terminal

Use this command to run Docker hello-world image

```
docker run hello-world
```

## Login to Docker Hub

generate a token from docker hub or github container registry:

github:

-   go to settings
-   Click on developer settings at the bottom
-   Click on personal access tokens tab
-   Click on Tokens (classic)
-   Click on generate new Token (classic)
-   Enable the settings: write:packages and delete:packages
-   Give it a name then generate the token

docker hub:

-   click on the drop down near your user name on the top right
-   click account settings
-   click on security then new access token
-   name it then generate one

Run this command in the terminal:

```
docker login
```

Enter your username for either github container registry or docker hub

Then you will enter the token you generated as the password

## Commands to start the project

All the commands you need to start and stop the project are here in this section.

Start the project by using this command to pull the built image and run it in a container:

```
docker compose up app-dev
```

Stop the project and remove the container created:

```
docker compose down app-dev
```

`Note: After running docker compose down the image you pulled will still exist on your local computer`

For production you just replace app-dev with app-prod
