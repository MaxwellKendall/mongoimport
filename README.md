# Import Collections into Mongo Atlas

MongoDB has developed a tool for this specific use case called `mongoimport`. You can import the `JSON` documents into your hosted instance of MongoDB using the following tutorials from MongoDB:

1. [Install MongoDB Tools](https://www.mongodb.com/docs/database-tools/installation/installation-macos/)
2. [Load File](https://www.mongodb.com/docs/atlas/import/mongoimport/)

```shell
mongoimport --jsonArray --uri "mongodb+srv://<dbUser>:<password>@<atlasUrl>/<databaseName>?retryWrites=true&w=majority" --collection <collectionName> --drop --file /some-json-file.json
```