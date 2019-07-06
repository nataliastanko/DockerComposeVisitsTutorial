## Docker Compose, Count Users Visits Tutorial

with multiple local isolated containers.

## Step 1.

### Node server setup & server code

Create ```package.json``` file.
Create ```index.js``` file.
Create ```Dockerfile``` file.

Run

    docker build .

Proceed to Step 2. if there are no errors.
Warnings (npm WARN) and notices (npm notice) are OK for now.

## Step 2.

Tag the image with name ```dockerUsername/projectname``` and tag ```latest```to not to have to work with IDs.

    docker build -t dockerUsername/projectname:latest .

Running 

    docker run dockerUsername/projectname

should work.

Create ```docker-compose.yml``` file.

Create and start instances of all containers, images, services list inside of ```docker-compose.yml``` file.

    docker-compose up

which is equivalent of ```docker run imageName```.

If any changes to the project images has been implemented, rebuild with

    docker-compose up --build

which is equivalent of ```docker build . && docker run imageName```.

To stop containers processes, run

    docker-compose down

## Step 3.

Go to [localhost:4001](http://localhost:4001/) to test visits counter.

***

***

***

* Based on [udemy course](https://www.udemy.com/docker-and-kubernetes-the-complete-guide/).
