## Query options
#### Matches documents with the key `price` with null and non-null values
```
db.inventory.find({"price":{$exists:true}});
```

#### Matches documents with the key `price` with non-null values
```
db.inventory.find({"price":{$ne:null}});
```

#### Matches documents with the key `price` with null values and documents without the key `price`
```
db.inventory.find({"price":null});
```

#### Matches values in an array
```
db.inventory.find( { status: { $in: [ "shirt", "trousers" ] } } )
```

