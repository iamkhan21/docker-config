dev: # Start development container
	docker-compose -f ./docker-compose.dev.yml up -V

dev_rebuild:
	docke-compose -f ./docker-compose.dev.yml up -V --build

dev-rebuild: dev_rebuild
dev_r: dev_rebuild
dev-r: dev_rebuild

prod: # Start production container on host
	docker-compose -f ./docker-compose.prod.yml up -d

update: # Update docker images
	docker-compose -f ./docker-compose.prod.yml pull

prod_rebuild: update
	docker-compose -f ./docker-compose.prod.yml up -d --build

prod-rebuild: prod_rebuild
prod_r: prod_rebuild
prod-r: prod_rebuild
