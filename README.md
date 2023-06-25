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

```bash
$ unzip dvdrental.zip
$ PGPASSWORD=postgres pg_restore -U postgres -h localhost -p 15432 -d dvdrental dvdrental.tar
```
