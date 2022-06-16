#### Create a text index on the fields on which you want to search for keywords
```
db.products.createIndex({"description":"text"})
```

#### Search for keywords
```
db.products.find({$text:{$search:"regular fit jeans"}})
```
