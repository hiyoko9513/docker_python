#!make
-include .env

# init:
# 	mkdir -p ../${WORKDIR}
# init-django:
# 	@init
# 	jango-admin startproject ${WORKDIR}
# 	python ${WORKDIR}/manage.py migrate
# 	docker-compose up -d
build:
	docker-compose build --no-cache --force-rm
up:
	docker-compose up -d
up-build:
	docker-compose up -d --build
stop:
	docker-compose stop
down:
	docker-compose down
appa:
	docker-compose exec app bash
restart:
	@make down
	@make up