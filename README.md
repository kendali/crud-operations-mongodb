# MongoDB Cheat Sheat

### Basic Commands

* عرض جميع قواعد البيانات

> `show dbs`

* عرض قاعدة البيانات الحالية   

> `db`
* إنشاء أو تبديل قاعدة البيانات
> `use <DataBaseName>`
* مسح قاعدة البيانات
> `drop <DataBaseName>`
* إنشاء مجموعة
> `db.createCollection('collectionName')`
* عرض المجموعات
> `show collections`
* 















___
### CRUD Operations 


1. **إنشاء (إدراج):**
   لإنشاء أو إدراج مستند في مجموعة يُستخدم الأمر 
   **`insertOne`** أو **`insertMany`**

   ```javascript
   db.collectionName.insertOne({ field1: قيمة1, field2: قيمة2 });

   db.collectionName.insertMany([{ field1: قيمة1 }, { field2: قيمة2 }]);
   ```

2. **قراءة (استعلام):**
   لقراءة أو استعلام المستندات من مجموعة  يُستخدم الأمر 
   **`find`**

   ```javascript
   db.collectionName.find();

   db.collectionName.find({ field: قيمة });

   db.collectionName.findOne({ _id: ObjectId("معرف_المستند") });
   ```

3. **تحديث:**
   لتحديث المستندات في مجموعة يُستخدم الأمر 
   **`updateOne`** أو **`updateMany`**

   ```javascript
   db.collectionName.updateOne({ filter }, { $set: { field: قيمة_جديدة } });

   db.collectionName.updateMany({ filter }, { $set: { field: قيمة_جديدة } });
   ```

4. **حذف:**
   لحذف المستندات من مجموعة MongoDB، يُستخدم الأمر 
   **`deleteOne`** أو **`deleteMany`**

   ```javascript
   db.collectionName.deleteOne({ filter });

   db.collectionName.deleteMany({ filter });
   ```









