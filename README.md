## notes on using MangoDB on macOS
### 1. Installation
```bash
$ brew install mongodb
```
### 2. Initialization
open one terminal.
```bash
$ cd ~/Documents/
$ mkdir mongoDB_db
$ mongod --dbpath mongoDB_db/
```
### 3. Connection
open anorther terminal.
```bash
$ mongo
> show dbs
# admin  0.000GB
# local  0.000GB
# test   0.000GB
> use test
# switched to db test
> show collections
# cats
> db.cats.find()
# { "_id" : ObjectId("5a08b8692efbed07afed8c7b"), "age" : 3, "name" : "Zildjian", "friends" : [ "tom", "jerry" ], "__v" : 0 }
```
