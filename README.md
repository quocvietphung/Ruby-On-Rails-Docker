# README

Learn how to use docker / docker compose to create and run rails application.

[Episode video link](https://youtu.be/a-jcTib9ZPA)

[![Episode Video Link](https://i.ytimg.com/vi/a-jcTib9ZPA/hqdefault.jpg)](https://youtu.be/a-jcTib9ZPA)

## Tested on

* Mac OSX - 10.10.5
* Docker - 1.12.1
* Docker compose - 1.8.0

## Instructions / commands

```
mkdir ~/projects/noteapp
cd ~/projects/noteapp
# Create Gemfile
# Create Dockerfile
# Create docker-compose.yml
docker-compose run app rails new . --force --database=mysql --skip-bundle
docker-compose build
docker-compose up
# http://localhost:3000

docker-compose run --rm app rails g scaffold note title body:text
docker exec web

Database command 
docker exec web rails mysql -uroot -p
docker exec web rails db:migrate || rails db:migrate



