# docker-postgres-dvd-rental

## Usage

```bash
$ cp .env.example .env
$ docker compose up
```

```bash
$ PGPASSWORD=postgres psql -U postgres -d dvdrental -h localhost -p 15432
```

## Restore

Sample database from [postgresql tutorial](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/).

```bash
$ curl -LO https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip
$ unzip dvdrental.zip
$ PGPASSWORD=postgres pg_restore -U postgres -h localhost -p 15432 -d dvdrental dvdrental.tar
```
