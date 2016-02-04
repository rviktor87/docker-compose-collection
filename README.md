# docker-compose collection
I didn't find appropiate docker-compose file for a lemp stack, which is separating the php, nginx, mysql applications.
So I created one :)

It's a good starting point for creating a distributed, load balanced, HA system.

# Requirements

Install [Docker](https://www.docker.io/) and [Compose](http://docs.docker.com/compose/install/)

I tried out with Docker 1.9.* >=

# Usage

`cd docker-compose-lemp`

`docker-compose up -d`
