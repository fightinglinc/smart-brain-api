# smart-brain-api
Install packages:
`npm install`

Run the server:
`node server.js`

Use PostgreSQL in the backend:
```SQL
CREATE TABLE users (
    id serial PRIMARY KEY,
    name VARCHAR(100),
    email text UNIQUE NOT NULL,
    entries BIGINT DEFAULT 0,
    joined TIMESTAMP NOT NULL
);
CREATE TABLE login (
    id serial PRIMARY KEY,
    hash varchar(100) NOT NULL,
    email text UNIQUE NOT NULL
);
```
