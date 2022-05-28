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
db.inventory.find( { "product_name": { $in: [ "shirt", "trousers" ] } } )
```

#### Matches values not in an array
```
db.inventory.find( { "product_name": { $nin: [ "shirt", "trousers" ] } } )
```

#### Less Than	`50`
```
db.inventory.find({"price":{$lt:50}})
```

#### Less Than Equals	`50`
```
db.inventory.find({"price":{$lte:50}})
```

#### Greater Than	`50`
```
db.inventory.find({"price":{$gt:50}})
```

#### Greater Than Equals	`50`
```
db.inventory.find({"price":{$gte:50}})
```

#### Not Equals	`50`
```
db.inventory.find({"price":{$ne:50}})
```

#### AND
```
db.inventory.find({$and:[{"product_name":"shirts"},{"price": {$ne:50}]})
```

#### OR
```
db.inventory.find({$or:[{"product_name":"shirts"},{"price": {$ne:50}]})
```

#### NOR
```
db.inventory.find({$nor:[{"product_name":"shirts"},{"price": {$ne:50}]})
```

#### NOT
```
db.inventory.find({$not:{"price": {$gt:50}}})
```
