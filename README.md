# docker-compose-snippets

### PostgreSQL
```bash
psql --username=postgres --dbname=postgres
# The same as
psql -U postgres -d postgres
```

Use docker image with the next command to create new user, providing non-default values

```bash
docker run
	--name <container-name>
	-p 5432:5432
	-e POSTGRES_USER=<db_user>
	-e POSTGRES_PASSWORD=<db_password>
	-e POSTGRES_DB=<db_name>
	-d <docker_image_name>:<docker_image_version>

```

