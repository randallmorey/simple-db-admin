## Start MongoDB in Docker:

From within this project:

```
docker-compose up mongo
```


## Run an Admin

In a separate terminal, clone the [admin mongo][admin-mongo] project and
install dependencies:

```
git clone https://github.com/mrvautin/adminMongo.git admin-mongo
cd admin-mongo
npm install
```

Start the admin:

```
npm start
```

Visit the admin at `http://0.0.0.0:1234`.


## Connections

In the admin, create a new named connection to the Mongo instance running in
Docker.  Use the connection string:  `mongodb://localhost:27017`.


## Databases

Navigate to `http://0.0.0.0:1234/app/connection` and create a new database
called `test`.  Navigate to the `test` collection to start editing data:
`http://0.0.0.0:1234/app/connection/test/test`.


[admin-mongo]: https://github.com/mrvautin/adminMongo
