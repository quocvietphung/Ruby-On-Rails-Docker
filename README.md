# README

Learn how to use docker / docker compose to create and run rails application.

## Instructions / commands

```
# Create Gemfile
# Create Dockerfile
# Create docker-compose.yml
docker-compose run app rails new . --force --database=mysql --skip-bundle
docker-compose build
docker-compose up

# http://localhost:3000
docker-compose run --rm app rails g scaffold note title body:text
docker exec web

# Database command 
docker exec web rails db:migrate
rails db:migrate



