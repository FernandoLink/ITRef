***
mongosh

db.help()
sh.help() - *sharding*
rs.help() - *replica*

show databases
use database
db.createCollection("collection")
show collections
db.collection.drop()
db.dropDatabase()
db.collection.insertOne(json)
db.collection.insertMany([json])
db.collection.find({filter},{projection}).sort({}).limit(5)
db.collection.find().pretty()
db.collection.updateOne(filter,json)
db.collection.updateMany(filter,[json])
db.collection.replaceOne(filter,json)
db.collection.deleteOne(filter)
db.collection.deleteMany(filter)


***
*Docker*

* docker run -d -p 27017:27017 --name my_mongodb -e MONGO_INITDB_ROOT_USERNAME=root -e MONGO_INITDB_ROOT_PASSWORD=pass mongo
* mongosh -u root -p pass --authenticationDatabase admin
* db.getMongo()
* mongodb://root:pass@127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&authSource=admin&appName=mongosh+1.8.0
***

##### SITES
***
[Operators](https://www.mongodb.com/docs/manual/reference/operator/query/)
