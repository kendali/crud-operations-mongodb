# CRUD Operations MongoDB

1. **Create (Insert):**
   To create or insert a document into a MongoDB collection, you use the `insertOne` or `insertMany` method.

   ```javascript
   db.collectionName.insertOne({ field1: value1, field2: value2 });

   db.collectionName.insertMany([{ field1: value1 }, { field2: value2 }]);
   ```

2. **Read (Query):**
   To read or query documents from a MongoDB collection, you use the `find` method.

   ```javascript
   db.collectionName.find();

   db.collectionName.find({ field: value });

   db.collectionName.findOne({ _id: ObjectId("documentId") });
   ```

3. **Update:**
   To update documents in a MongoDB collection, you use the `updateOne` or `updateMany` method.

   ```javascript
   db.collectionName.updateOne({ filter }, { $set: { field: newValue } });

   db.collectionName.updateMany({ filter }, { $set: { field: newValue } });
   ```

4. **Delete:**
   To delete documents from a MongoDB collection, you use the `deleteOne` or `deleteMany` method.

   ```javascript
   db.collectionName.deleteOne({ filter });

   db.collectionName.deleteMany({ filter });
   ```

