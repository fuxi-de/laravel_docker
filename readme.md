# Laravel Docker Environment

This is a Docker Environment meant for developing [Laravel](https://laravel.com/) Applications. It consists of 2 Services. The Core Service being an nginx Webserver running the Application, and an MySql 5.7 Service for the Database.

## Getting Started

To get started clone this Repository and inside create an Directory called __src__ on the same level as the __Docker__ Directory.

```shell
git clone https://github.com/fuxi-de/laravel_docker.git
cd laravel_docker
mkdir src
```

This Directory will get mounted into the Core Container so your Laravel Application will live inside it.

After creating a Laravel App inside the __src__ Directory either by using __laravel new__ command or cloning from Version control or whatever floats your boat :P, you can boot up the Docker Containers by running:

```shell
docker-compose up
```

If there aren't any errors you should be able to reach your Laravel App under [http://localhost:8080](http://localhost:8080). Of course you can swap out the Port you want to use in the Dockerfile.
