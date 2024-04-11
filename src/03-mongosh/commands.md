# Comandos para la shell de MongoDB

Mongo SH es el cli de Mongo y sirve para conectarnos a mongo atlas o a nuestra base de datos local y no necesitamos instalar nada solo correr nuestro contenedor.

## Connect to container

```sh
    docker-compose exec mongodb bash
```

## Connect with mongosh

```sh
    mongosh "mongodb+srv://usuario:contraseña@cluster101.qk4sjo5.mongodb.net/"
    mongosh "mongodb://usuario:contraseña@@localhost:27017"
```

```sh
    show dbs
    show collections
```

Tambien puedo ejecutar scripts

```js
    use('sample_training')

    db.zips.find({'state': 'NY'}).count()
```
