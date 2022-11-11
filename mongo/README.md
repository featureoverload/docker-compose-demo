# Mongo, docker-compose-demo

## Usage

```shell
$ docker-compose up -d
```

```shell
$ docker-compose exec mongo bash
root@008b82d44130:/# mongo $DB_DATABASE -u $DB_USERNAME -p $DB_PASSWORD
MongoDB shell version v4.2.22
connecting to: mongodb://127.0.0.1:27017/new_db?compressors=disabled&gssapiServiceName=mongodb
Implicit session: session { "id" : UUID("7548054e-89b0-4ef9-8247-ffa2af70d859") }
MongoDB server version: 4.2.22
Welcome to the MongoDB shell.
For interactive help, type "help".
For more comprehensive documentation, see
        https://docs.mongodb.com/
Questions? Try the MongoDB Developer Community Forums
        https://community.mongodb.com
> db.item.find()
{ "_id" : ObjectId("636dd853453f2ddcfa3350f0"), "title" : "setup-db", "description" : "initialize when mongo container up" }
{ "_id" : ObjectId("636dd853453f2ddcfa3350f1"), "title" : "hello", "description" : "testing" }
{ "_id" : ObjectId("636dd853453f2ddcfa3350f2"), "title" : "fuzzbuzz", "description" : "eggspam" }
> exit
bye
root@008b82d44130:/# exit
exit
$
```
