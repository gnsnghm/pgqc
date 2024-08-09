# pgqc(PostGresql Query Comparison tool)

## How to use

copy `backend/config.json.example`

`cp backend/config.json.example backend/config.json`

edit `backend/config.json`

### About config.json

- Please refer to config.json.example for input
- You can set one or multiple configurations
- Separate by commas
- The items to be set are `dbname`, `user`, `password`, `host`, `port`
    - `dbname`: Name of the database
    - `user`: Connection username
    - `password`: Password for the connection user
    - `port`: Port number
- If you cannot connect, check if the connection is allowed in `pg_hba.conf` at the destination
- If you still cannot connect, check if `listen_address` is allowed in `postgresql.conf`

## How to run

`dokcer compose up -d`
