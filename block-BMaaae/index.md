writeCode

Write code to:-

- create a database named `sports`.
  use sports //
- list all databases present in local mongod server.
  show dbs
- create 3 collections named `cricket`, `football`, `TT` in sports databse.
  db.createCollection("cricket")
  db.createCollection("football")
  db.createCollection("TT")
- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
  db.cricket.insertMany([{name : "Aman", age : 23, email : "aman@gmail.com", bid_price : 25000}])

- list all collections in sports database.
  show collections
- rename `TT` collection to `tennis`.
  db.TT.renameCollection("tennis")
- create a capped collection called `khokho` which should have max 3 documents.
  db.createCollection("khokho")
  Try inserting more than 3 and see what happens?
- check whether a collection is capped or not?
- drop all documents from `football` collection.
  db.football.remove({})
- delete cricket collection completely.
  db.cricket.drop()
- delete sports database.
  db.dropDatabase()
- check which database you are connected to ?
  db
- connect to test database
  use test
