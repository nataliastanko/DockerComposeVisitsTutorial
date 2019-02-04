## Docker Compose Visits Tutorial

with multiple local isolated containers

## Step 1.

Run

    docker build .

Tag docker image

    docker build -t nataliastanko/vists:latest .

## Step 2.

Run

    docker-compose up

If any changes to the project has been implemented, rebuild with

    docker-compose up --build

To stop containers, run

    docker-compose down

***

***

***

* Based on [udemy course](https://www.udemy.com/docker-and-kubernetes-the-complete-guide/).
