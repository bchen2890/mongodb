## Relationships
#### Modeling Embedded Relationships
##### User Collection
```
{
	 "_id":ObjectId("52ffc33cd85242f436185947"),
   "username": "bchen",
   "addresses": [{
              "street": "Main Street",
              "city": "Madrid",
              "zip": "12345"
            }]
}
```

#### Modeling Referenced Relationships
##### User Collection
```
{
	 "_id":ObjectId("52ffc33cd85242f436185947"),
   "username": "bchen",
   "addresses": [ObjectId("52ffc33cd85242f436185900")]
}
```
##### Address Collection
```
{
	 "_id":ObjectId("52ffc33cd85242f436185900"),
    "street": "Main Street",
    "city": "Madrid",
    "zip": "12345"
}
```
