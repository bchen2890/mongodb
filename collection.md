## Collection commands

#### Insert a document
```
db.User.insertOne({"username":"bchen"})
```
#### Insert multiple documents
```
db.User.insertMany([{"username":"bchen"},{"username":"mgdb"}])
```

#### List all documents
```
db.User.find()
```
#### Filter documents
```
db.User.find({"username":/b/})
```

#### Count documents
```
db.User.countDocuments()
```

#### Remove a document
```
db.User.deleteOne({"username":"bchen"})
```
#### Remove multiple documents
```
db.User.deleteMany({"username": /b/})
```
