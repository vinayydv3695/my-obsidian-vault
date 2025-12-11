---
tags: 
timestamp: "2025-12-12T01:25:07+05:30"
---

### **Topic: Introduction & Fundamentals of NoSQL**

**1. What does "NoSQL" typically stand for?**  
A. No SQL Allowed  
B. Not Only SQL  
C. Non-Structured Query Language  
D. New SQL Design  
**Answer: B**

**2. Which of the following is a primary characteristic of NoSQL databases?**  
A. Fixed Schema  
B. Vertical Scalability  
C. Schema Flexibility  
D. Complex Joins  
**Answer: C**

**3. In the context of RDBMS vs. NoSQL, what does "Vertical Scaling" typically refer to?**  
A. Adding more servers to a cluster  
B. Adding more power (CPU/RAM) to a single server  
C. Distributing data across regions  
D. Creating more tables  
**Answer: B**

**4. NoSQL databases are generally designed to support which type of scaling?**  
A. Horizontal Scaling  
B. Vertical Scaling  
C. Diagonal Scaling  
D. Manual Scaling  
**Answer: A**

**5. Which of the following best describes the data structure of a NoSQL database?**  
A. Always tables with rows and columns  
B. Strictly graph-based  
C. A single data structure like key-value, document, or graph  
D. Spreadsheets  
**Answer: C**

**6. Why might a company choose NoSQL over RDBMS for a web application?**  
A. To enforce strict ACID compliance  
B. To handle large volumes of unstructured data with a flexible schema  
C. Because they have very little data  
D. To use complex joins frequently  
**Answer: B**

**7. Which data model organizes data into "Collections" and "Documents"?**  
A. Key-Value Store  
B. Relational Database  
C. Document Database  
D. Graph Database  
**Answer: C**

**8. In a Grocery Shop scenario, which challenge with RDBMS involves difficulty in handling new data models after a company acquisition?**  
A. Team Challenge  
B. Company Expansion  
C. Company Acquisition  
D. Multiple Vendors  
**Answer: C**

**9. What is the primary downside of RDBMS when data volume grows extremely large?**  
A. It cannot store numbers  
B. Scaling is difficult and expensive (usually vertical)  
C. It does not support SQL  
D. It loses data automatically  
**Answer: B**

**10. Which feature is generally NOT a strength of NoSQL databases?**  
A. Horizontal Scalability  
B. Flexible Schema  
C. Complex Joins  
D. High Availability  
**Answer: C**

---

### **Topic: Types of NoSQL Databases**

**11. Which NoSQL database type stores data as a dictionary or map?**  
A. Document Store  
B. Column Family  
C. Key-Value Store  
D. Graph Database  
**Answer: C**

**12. Redis and DynamoDB are examples of which type of NoSQL database?**  
A. Document  
B. Key-Value  
C. Graph  
D. Column-Oriented  
**Answer: B**

**13. Which database type is best suited for "Session Caching" or "Shopping Cart" data?**  
A. Graph Database  
B. Key-Value Store  
C. RDBMS  
D. Document Database  
**Answer: B**

**14. What is the primary data unit in a Document Database (like MongoDB)?**  
A. Row  
B. Node  
C. JSON/BSON Document  
D. Column Family  
**Answer: C**

**15. Apache Cassandra and HBase are examples of:**  
A. Key-Value Stores  
B. Document Databases  
C. Graph Databases  
D. Column-Oriented Databases  
**Answer: D**

**16. Which database type is ideal for "Social Network" relationships?**  
A. Key-Value  
B. Document  
C. Graph  
D. Column-Oriented  
**Answer: C**

**17. In a Graph Database, what are the entities (like people) called?**  
A. Edges  
B. Nodes  
C. Keys  
D. Tables  
**Answer: B**

**18. In a Graph Database, what are the relationships between entities called?**  
A. Edges  
B. Vertices  
C. Rows  
D. Collections  
**Answer: A**

**19. Neo4j is a popular example of which database type?**  
A. Document  
B. Graph  
C. Key-Value  
D. Column-Oriented  
**Answer: B**

**20. Which database type is best for storing "Time Series" data?**  
A. Key-Value  
B. Graph  
C. Column-Oriented  
D. Document  
**Answer: C**

**21. MongoDB uses which format to store documents?**  
A. CSV  
B. JSON/BSON  
C. HTML  
D. Plain Text  
**Answer: B**

**22. Which database is known for handling "Massive Writes" efficiently?**  
A. Redis  
B. Neo4j  
C. Cassandra  
D. MySQL  
**Answer: C**

**23. Which use case is NOT ideal for a Key-Value store?**  
A. User Profiles  
B. Session Management  
C. Managing complex relationships between millions of users  
D. Product recommendations  
**Answer: C**

**24. Which type of database allows "Nested Data" structures easily?**  
A. Key-Value  
B. Document  
C. RDBMS  
D. Graph  
**Answer: B**

**25. Amazon Neptune is an example of:**  
A. Key-Value Store  
B. Document Store  
C. Graph Database  
D. Relational Database  
**Answer: C**

---

### **Topic: ACID vs. BASE**

**26. What does the "A" in ACID stand for?**  
A. Availability  
B. Atomicity  
C. Accuracy  
D. Authorization  
**Answer: B**

**27. What does the "C" in ACID stand for?**  
A. Consistency  
B. Capacity  
C. Cloud  
D. Connectivity  
**Answer: A**

**28. Which acronym describes the properties of most NoSQL databases?**  
A. ACID  
B. SOLID  
C. BASE  
D. CRUD  
**Answer: C**

**29. What does "Soft state" in BASE mean?**  
A. The system is physically soft  
B. The state may change over time, even without input  
C. The database is read-only  
D. Data is deleted automatically  
**Answer: B**

**30. "Eventual Consistency" implies that:**  
A. The database is never consistent  
B. The database is strictly consistent  
C. The database may be inconsistent briefly but becomes consistent eventually  
D. Data is saved only sometimes  
**Answer: C**

**31. RDBMS transactions typically strictly follow which model?**  
A. BASE  
B. ACID  
C. CAP  
D. SOAP  
**Answer: B**

**32. "Basic Availability" in BASE guarantees:**  
A. System is available 50% of the time  
B. Each request gets a response (success or failure)  
C. Only read requests allowed  
D. Strong consistency maintained  
**Answer: B**

**33. Durability in ACID ensures:**  
A. Transactions are fast  
B. Completed transactions persist after restart  
C. Users access data globally  
D. Database never crashes  
**Answer: B**

---

### **Topic: RDBMS vs. NoSQL Comparison**

**34. In RDBMS, how are relationships typically handled?**  
A. Nesting data  
B. Foreign Keys  
C. Graph Edges  
D. Not handled  
**Answer: B**

**35. How does MongoDB typically handle relationships?**  
A. Foreign Keys  
B. Joins only  
C. Embedding or Referencing  
D. No relationships allowed  
**Answer: C**

**36. If you delete a record in RDBMS with "ON DELETE CASCADE", what happens?**  
A. Only parent deleted  
B. Child records automatically deleted  
C. DB stops working  
D. It asks for password  
**Answer: B**

**37. How is related data deletion handled in MongoDB?**  
A. Automatic Cascade Delete  
B. DB deletes it later  
C. Manual delete or embedded data  
D. Impossible  
**Answer: C**

**38. Which type of queries are RDBMS generally good for?**  
A. Unstructured text search  
B. Normalized queries  
C. Graph traversals  
D. JSON parsing  
**Answer: B**

**39. RDBMS schemas are:**  
A. Dynamic  
B. Flexible  
C. Fixed  
D. Optional  
**Answer: C**

**40. Which DB is better for denormalized data?**  
A. MySQL  
B. PostgreSQL  
C. MongoDB  
D. Oracle  
**Answer: C**

---

### **Topic: Case Studies & Migration**

**41. Which database did Netflix migrate to from Oracle?**  
A. MongoDB  
B. MySQL  
C. Cassandra  
D. Neo4j  
**Answer: C**

**42. Why did Netflix move to AWS + Cassandra?**  
A. Reduce costs  
B. Massive scalability for global users  
C. Oracle failed  
D. Wanted Graph DB  
**Answer: B**

**43. Twitter uses MySQL + which NoSQL DB for caching/timeline?**  
A. Neo4j  
B. Redis  
C. Oracle  
D. SQLite  
**Answer: B**

**44. In the Grocery Shop case, what was a team challenge?**  
A. They demanded money  
B. New devs struggled due to complex RDBMS design  
C. They didn't know SQL  
D. They preferred ledgers  
**Answer: B**

**45. When providing APIs to aggregators, what issue arose?**  
A. Data too small  
B. Needed flexible retrieval, hard with rigid RDBMS  
C. APIs not supported  
D. Internet issue  
**Answer: B**

**46. Which NoSQL feature solves the “Company Acquisition” challenge?**  
A. Fixed schema  
B. ACID  
C. Schema flexibility  
D. Foreign Keys  
**Answer: C**

---

### **Topic: General & Syntax**

**47. If you insert a document into a non-existent collection in MongoDB:**  
A. Error  
B. Collection auto-created  
C. Crash  
D. Ignored  
**Answer: B**

**48. Command to insert multiple documents:**  
A. `db.collection.addMany()`  
B. `db.collection.insertMany()`  
C. `db.collection.saveAll()`  
D. `db.collection.push()`  
**Answer: B**

**49. How to represent One-to-Many in Document DB for fast reads?**  
A. Two tables  
B. Join  
C. Embed array inside User  
D. Graph edge  
**Answer: C**

**50. Command to decrease stock by 2:**  
A. `{$set: {stock: -2}}`  
B. `{$minus: {stock: 2}}`  
C. `{$inc: {stock: -2}}`  
D. `{$dec: {stock: 2}}`  
**Answer: C**

**51. Operator for Greater than or equal to:**  
A. `$gt`  
B. `$ge`  
C. `$gte`  
D. `$e`  
**Answer: C**

**52. Default index in MongoDB:**  
A. name  
B. email  
C. _id  
D. date  
**Answer: C**

**53. Aggregation stage to flatten array:**  
A. `$group`  
B. `$project`  
C. `$unwind`  
D. `$match`  
**Answer: C**

**54. Why does Twitter use both MySQL & NoSQL?**  
A. Couldn't decide  
B. Consistency + Scalability combo  
C. MySQL for images  
D. NoSQL for login only  
**Answer: B**

**55. Which DB uses Cypher Query Language?**  
A. MongoDB  
B. Cassandra  
C. Neo4j  
D. Redis  
**Answer: C**

**56. "Wide Column" stores are also known as:**  
A. Document Stores  
B. Column Family Databases  
C. Graph Stores  
D. XML Databases  
**Answer: B**

**57. Node in MongoDB replica set that accepts writes:**  
A. Secondary  
B. Arbiter  
C. Primary  
D. Hidden  
**Answer: C**

**58. Which is NOT a NoSQL category?**  
A. Key-Value  
B. Document  
C. Spreadsheet-based  
D. Graph  
**Answer: C**

**59. If schema needs to evolve over time, best DB is:**  
A. RDBMS  
B. NoSQL (Document)  
C. Flat File  
D. Directory Service  
**Answer: B**

**60. Command to initiate a Replica Set:**  
A. `rs.start()`  
B. `rs.initiate()`  
C. `rs.begin()`  
D. `rs.create()`  
**Answer: B**

### **Unit 2: Introduction, Architecture, and Installation**

**61. Which NoSQL database type is best suited for storing relationships between data entities, such as social networks?**  
A. Document Store  
B. Column-Family Store  
C. Graph Store  
D. Key-Value Store  
**Answer: C**

**62. Which of the following is NOT a characteristic of MongoDB?**  
A. Schema-less (Flexible Schema)  
B. Uses BSON format for storage  
C. Supports complex Joins natively like SQL  
D. Horizontal Scalability  
**Answer: C**

**63. What is the default TCP port that MongoDB listens on?**  
A. 3306  
B. 8080  
C. 27017  
D. 5432  
**Answer: C**

**64. Which command is used to start the MongoDB server process?**  
A. mongo  
B. mongosh  
C. mongod  
D. start-mongo  
**Answer: C**

**65. By default, on Windows, where does MongoDB attempt to store data files?**  
A. C:\Program Files\MongoDB\data  
B. C:\data\db  
C. /var/lib/mongo  
D. C:\mongo\data  
**Answer: B**

**66. Which file format does `mongodump` create by default?**  
A. JSON  
B. CSV  
C. Binary (BSON)  
D. SQL Dump  
**Answer: C**

**67. Which tool would you use to import a JSON or CSV file into MongoDB?**  
A. mongorestore  
B. mongoimport  
C. mongoload  
D. bsondump  
**Answer: B**

**68. What is the primary purpose of the `bsondump` tool?**  
A. Convert BSON dump files into readable JSON  
B. Delete the database  
C. Encrypt database backups  
D. Import binary data  
**Answer: A**

**69. Which command tracks the amount of time a MongoDB instance spends reading and writing data, refreshing every second?**  
A. db.stats()  
B. mongostat  
C. mongotop  
D. db.serverStatus()  
**Answer: C**

**70. In a Document database, what is the equivalent of a "Table" in RDBMS?**  
A. Document  
B. Collection  
C. Field  
D. View  
**Answer: B**

**71. Which scaling strategy does MongoDB primarily use to handle massive data loads?**  
A. Vertical Scaling  
B. Horizontal Scaling (Sharding)  
C. Normalization  
D. Stored Procedures  
**Answer: B**

**72. What does BSON stand for?**  
A. Basic JSON  
B. Binary JSON  
C. Big JSON  
D. Backend JSON  
**Answer: B**

**73. Which of the following is a Column-Family database?**  
A. Redis  
B. MongoDB  
C. Cassandra  
D. Neo4j  
**Answer: C**

**74. Which utility restores a backup created by `mongodump`?**  
A. mongoimport  
B. mongorestore  
C. db.restore()  
D. mongoexport  
**Answer: B**

**75. If you run `mongoexport` without specifying format, what is the default output?**  
A. CSV  
B. BSON  
C. JSON  
D. XML  
**Answer: C**

---

### **Unit 3: Querying, Modifiers, and Indexing**

**76. What happens if you insert a document into a collection that does not exist?**  
A. Error  
B. Waits for admin  
C. MongoDB auto-creates the collection  
D. Discarded  
**Answer: C**

**77. Which method inserts multiple documents at once?**  
A. addMany  
B. insertMany  
C. saveMany  
D. putAll  
**Answer: B**

**78. Default value of `ordered` in `insertMany`?**  
A. true  
B. false  
C. null  
D. 1  
**Answer: A**

**79. If `insertMany` with ordered:true errors on 3rd of 5 docs:**  
A. All rollback  
B. First 2 saved, then stops  
C. First 2 saved, continues  
D. Retries  
**Answer: B**

**80. Operator to increment a value?**  
A. $add  
B. $sum  
C. $inc  
D. $plus  
**Answer: C**

**81. Operator to add to array only if value not present?**  
A. $push  
B. $addToSet  
C. $append  
D. $addUnique  
**Answer: B**

**82. `$pop` value to remove last item from array?**  
A. -1  
B. 0  
C. 1  
D. "last"  
**Answer: C**

**83. Operator to push multiple values at once?**  
A. $all  
B. $many  
C. $each  
D. $list  
**Answer: C**

**84. `$slice` with `$push` does what?**  
A. Cuts array  
B. Limits array length  
C. Sorts array  
D. Removes specific values  
**Answer: B**

**85. Method returning a cursor?**  
A. findOne  
B. get  
C. find  
D. search  
**Answer: C**

**86. In `find().sort().limit().skip()`, which logically happens first?**  
A. limit  
B. skip  
C. sort  
D. Left-to-right  
**Answer: C**

**87. Query for age > 25?**  
A. { age: { $gt: 25 } }  
B. { age: { $more: 25 } }  
C. { age: > 25 }  
D. { age: { $gte: 25 } }  
**Answer: A**

**88. Command to delete all matching documents?**  
A. removeOne  
B. deleteAll  
C. deleteMany  
D. drop  
**Answer: C**

**89. Default index created automatically?**  
A. name  
B. _id  
C. created_at  
D. timestamp  
**Answer: B**

**90. Index for sphere-based geometric queries?**  
A. 2d  
B. geoHaystack  
C. 2dsphere  
D. 3d  
**Answer: C**

**91. Compound index on user asc, date desc?**  
A. { user:1, date:1 }  
B. { user:1, date:-1 }  
C. ensureIndex asc/desc  
D. addIndex  
**Answer: B**

**92. What is an Index Prefix?**  
A. First character of index name  
B. Subset of fields at beginning of compound index  
C. Setting for text index  
D. Partial value index  
**Answer: B**

**93. Which ensures no duplicate values in an indexed field?**  
A. sparse:true  
B. distinct:true  
C. unique:true  
D. primary:true  
**Answer: C**

**94. Sparse Index contains:**  
A. Only documents that have the indexed field  
B. Only documents without it  
C. All docs but compressed  
D. Only unique docs  
**Answer: A**

**95. Which index auto-removes documents after time?**  
A. Hashed  
B. TTL  
C. Sparse  
D. Timer  
**Answer: B**

**96. Method to view execution plan?**  
A. plan  
B. stats  
C. explain  
D. analyze  
**Answer: C**

**97. `.hint()` does what?**  
A. Suggests query writing  
B. Forces use of a specific index  
C. Hides fields  
D. Comments code  
**Answer: B**

**98. Command to rename namespace or drop index during restore?**  
A. --rename  
B. --nsFrom / --nsTo  
C. --changeNamespace  
D. --switchDB  
**Answer: B**

**99. MongoDB version introducing multi-document transactions?**  
A. 3.2  
B. 3.6  
C. 4.0  
D. 5.0  
**Answer: C**

**100. Default max execution time for a transaction?**  
A. 30 sec  
B. 60 sec  
C. 5 min  
D. Unlimited  
**Answer: B**

**101. Isolation level used in MongoDB transactions?**  
A. Read Uncommitted  
B. Snapshot Isolation  
C. Serializable  
D. Repeatable Read  
**Answer: B**

**102. Object required before starting a transaction?**  
A. Client  
B. Session  
C. TransactionID  
D. Lock  
**Answer: B**

**103. Mechanism ensuring durability via logged operations?**  
A. Journal  
B. Oplog  
C. Config Server  
D. Arbiter  
**Answer: B**

**104. Profiler level logging all operations?**  
A. 0  
B. 1  
C. 2  
D. 3  
**Answer: C**

**105. Profiler stores data where?**  
A. OS log file  
B. system.profile collection  
C. admin.logs  
D. RAM  
**Answer: B**

**106. Key characteristic of `system.profile` collection?**  
A. Temporary  
B. Capped Collection  
C. Read-only  
D. Hidden  
**Answer: B**

**107. `$jsonSchema` is used to:**  
A. Convert BSON to JSON  
B. Enforce schema validation  
C. Export data  
D. Query strings  
**Answer: B**

**108. Syntax to remove field `favBook`?**  
A. $delete  
B. $remove  
C. $unset  
D. $set null  
**Answer: C**

**109. In compound index `{ a:1, b:1 }`, which query cannot use index efficiently?**  
A. find({a:5})  
B. find({a:5, b:6})  
C. find({b:6})  
D. find({a:5}).sort({b:1})  
**Answer: C**

**110. Purpose of `mongodump --oplog`?**  
A. Dump logs only  
B. Create point-in-time snapshot  
C. Backup logic  
D. Faster dump  
**Answer: B**

**111. Which Replica Set node accepts writes?**  
A. Secondary  
B. Arbiter  
C. Primary  
D. Hidden  
**Answer: C**

**112. `2d` index supports:**  
A. Spherical queries  
B. Flat planar geometry  
C. Full-text search  
D. 3D modeling  
**Answer: B**

**113. Command to rebuild all indexes on a collection?**  
A. reIndex  
B. fixIndex  
C. repair  
D. buildIndex  
**Answer: A**

**114. `mongoexport` is best suited for:**  
A. Full backups  
B. Moving small JSON/CSV datasets  
C. Disaster recovery  
D. Backing up indexes  
**Answer: B**

**115. Query to find documents where `tags` contains both "red" and "blue"?**  
A. { tags: "red", tags: "blue" }  
B. { tags: { $in: ["red","blue"] } }  
C. { tags: { $all: ["red","blue"] } }  
D. { tags: { $both: ["red","blue"] } }  
**Answer: C**

**116. Command to check profiling status?**  
A. db.getProfilingStatus()  
B. db.profiler.status()  
C. show profile  
D. db.status()  
**Answer: A**

**117. Operator to convert string to uppercase?**  
A. $upper  
B. $toUpper  
C. $uppercase  
D. $caps  
**Answer: B**

**118. What happens if unique index is created but duplicates exist?**  
A. Creates index and deletes duplicates  
B. Creates index and ignores duplicates  
C. Index creation fails  
D. Merges duplicates  
**Answer: C**

**119. Index required for `$text` search?**  
A. Single Field  
B. Text Index  
C. String Index  
D. Multikey  
**Answer: B**

**120. MongoDB Atomicity guarantees:**  
A. Single document operations are all-or-nothing  
B. Reads always from primary  
C. DB never crashes  
D. Data always normalized  
**Answer: A**

### **Unit 4: Aggregation & Sharding**

**121. What is the primary purpose of the MongoDB Aggregation Framework?**  
A. Enforce strict schema  
B. Process and transform documents within the server  
C. Manage authentication  
D. Perform backups  
**Answer: B**

**122. In an aggregation pipeline, what does the output of one stage become?**  
A. The final result  
B. Input for the next stage  
C. A new collection  
D. A BSON file  
**Answer: B**

**123. Which stage filters documents (similar to `find()`)?**  
A. $project  
B. $group  
C. $match  
D. $sort  
**Answer: C**

**124. Why place `$match` early in the pipeline?**  
A. Ensure sorted output  
B. Reduce documents processed by later stages  
C. Require JSON output  
D. Syntax requirement  
**Answer: B**

**125. Which stage reshapes documents (renaming fields, computing new ones)?**  
A. $match  
B. $project  
C. $unwind  
D. $limit  
**Answer: B**

**126. How to reference field "price" inside `$project`?**  
A. "price"  
B. price  
C. "$price"  
D. { price: 1 }  
**Answer: C**

**127. Which stage groups documents?**  
A. $sort  
B. $group  
C. $bucket  
D. $count  
**Answer: B**

**128. Mandatory field in `$group`?**  
A. key  
B. _id  
C. groupBy  
D. field  
**Answer: B**

**129. Which operator deconstructs arrays into multiple documents?**  
A. $split  
B. $arrayElemAt  
C. $unwind  
D. $extract  
**Answer: C**

**130. If array has 3 elements, `$unwind` outputs how many documents?**  
A. 1  
B. 3  
C. 0  
D. Error  
**Answer: B**

**131. Which stage writes aggregation result to a new collection (replacing existing)?**  
A. $save  
B. $merge  
C. $out  
D. $export  
**Answer: C**

**132. Which stage merges results into an existing collection (upsert)?**  
A. $merge  
B. $insert  
C. $combine  
D. $union  
**Answer: A**

**133. Operator to total numeric values in a group?**  
A. $count  
B. $add  
C. $sum  
D. $total  
**Answer: C**

**134. Operator returning highest value?**  
A. $top  
B. $high  
C. $max  
D. $peak  
**Answer: C**

**135. Stage used to perform left outer join?**  
A. $join  
B. $lookup  
C. $connect  
D. $unionWith  
**Answer: B**

**136. In `$lookup`, `localField` refers to:**  
A. Field in target collection  
B. Field in input documents  
C. Output array name  
D. Database name  
**Answer: B**

**137. Operator to join two strings?**  
A. $join  
B. $mergeString  
C. $concat  
D. $append  
**Answer: C**

**138. Correct order for efficient pagination?**  
A. limit → skip → sort  
B. skip → limit → sort  
C. sort → skip → limit  
D. sort → limit → skip  
**Answer: C**

**139. Operator to extract substring?**  
A. $slice  
B. $substr  
C. $cut  
D. $substring  
**Answer: B**

**140. Expression returning array size?**  
A. $length  
B. $count  
C. $size  
D. $width  
**Answer: C**

**141. How to exclude `_id` in `$project`?**  
A. _id: false  
B. _id: 0  
C. exclude: "_id"  
D. $remove: "_id"  
**Answer: B**

**142. Boolean NOT operator?**  
A. $nor  
B. $invert  
C. $not  
D. $negate  
**Answer: C**

**143. `$arrayElemAt` does what?**  
A. Returns array  
B. Returns element at index  
C. Returns first element  
D. Returns last element  
**Answer: B**

**144. Which is NOT a valid `$group` accumulator?**  
A. $sum  
B. $avg  
C. $push  
D. $match  
**Answer: D**

**145. Operator converting string to uppercase?**  
A. $upper  
B. $toUpper  
C. $capitalize  
D. $uppercase  
**Answer: B**

**146. Which allows computing new fields?**  
A. find()  
B. Aggregation  
C. Both  
D. Neither  
**Answer: B**

**147. MapReduce in modern MongoDB is:**  
A. Primary engine  
B. Deprecated  
C. Faster than Aggregation  
D. Only for graph data  
**Answer: B**

**148. `emit` takes how many arguments?**  
A. 1  
B. 2 (key, value)  
C. 3  
D. 0  
**Answer: B**

**149. Keyword referring to current document in Map?**  
A. doc  
B. current  
C. self  
D. this  
**Answer: D**

**150. What is Sharding?**  
A. Encrypting data  
B. Distributing data across multiple machines  
C. Creating backups  
D. Compressing data  
**Answer: B**

**151. Component routing queries to shards?**  
A. mongod  
B. mongos  
C. Config Server  
D. Arbiter  
**Answer: B**

**152. Chunk metadata stored where?**  
A. Shards  
B. Mongos  
C. Config Servers  
D. Client  
**Answer: C**

**153. What is a Shard Key?**  
A. Password  
B. Field used to partition data  
C. Config server key  
D. Unique index  
**Answer: B**

**154. Property describing number of unique shard key values?**  
A. Monotonicity  
B. Frequency  
C. Cardinality  
D. Density  
**Answer: C**

**155. Low cardinality shard key causes:**  
A. Too many chunks  
B. Jumbo chunks  
C. Excess memory  
D. Slow network  
**Answer: B**

**156. Monotonically increasing shard key causes:**  
A. Even writes  
B. Write hotspot on one shard  
C. Random distribution  
D. Faster reads  
**Answer: B**

**157. Strategy distributing docs via hash of key?**  
A. Range  
B. Hashed  
C. Tag-aware  
D. Zone  
**Answer: B**

**158. Range sharding is most efficient for:**  
A. Random lookups  
B. Range queries  
C. Text search  
D. Graph traversal  
**Answer: B**

**159. Default chunk size in MongoDB?**  
A. 1 MB  
B. 64 MB  
C. 1 GB  
D. 100 MB  
**Answer: B**

**160. Background process moving chunks for balance?**  
A. Replicator  
B. Arbiter  
C. Balancer  
D. Journaler  
**Answer: C**

**161. Each database has a ______ for unsharded collections.**  
A. Primary Shard  
B. Master Node  
C. Config Shard  
D. Backup Shard  
**Answer: A**

**162. Command to enable sharding on DB?**  
A. db.enableSharding()  
B. sh.enableSharding()  
C. rs.sharding()  
D. admin.shard()  
**Answer: B**

**163. Command to shard a collection?**  
A. db.collection.shard()  
B. sh.shardCollection()  
C. sh.addShard()  
D. db.partition()  
**Answer: B**

**164. In zoned sharding, data goes to shards based on:**  
A. Hash  
B. Defined ranges (tags)  
C. Size of documents  
D. Insert time  
**Answer: B**

**165. High frequency of a single shard key value produces:**  
A. Better compression  
B. Monolithic chunk  
C. Faster indexing  
D. Zero downtime  
**Answer: B**

**166. To perform text search, you must create:**  
A. Compound index  
B. Text index  
C. Hashed index  
D. Unique index  
**Answer: B**

**167. Operator used for text search:**  
A. $find  
B. $search  
C. $text  
D. $query  
**Answer: C**

**168. Search exact phrase "coffee shop"?**  
A. coffee shop  
B. \"coffee shop\"  
C. { phrase: "coffee shop" }  
D. ["coffee","shop"]  
**Answer: B**

**169. Exclude a term (e.g., sugar) in text search:**  
A. NOT sugar  
B. !sugar  
C. -sugar  
D. ^sugar  
**Answer: C**

**170. `$meta: "textScore"` represents:**  
A. Count  
B. Relevance score  
C. Document size  
D. Query time  
**Answer: B**

**171. In `$project`, "$field" means:**  
A. Literal "$field"  
B. Value of field  
C. Variable  
D. System command  
**Answer: B**

**172. When is `$` used as operator?**  
A. { $gt: 50 }  
B. "$price"  
C. "$name"  
D. { name: 1 }  
**Answer: A**

**173. When should you NOT use `$`?**  
A. Field name on left of filter  
B. Calculating sum  
C. Referencing field in projection  
D. Using $set  
**Answer: A**

**174. Accumulator adding unique values to array?**  
A. $push  
B. $addToSet  
C. $append  
D. $unique  
**Answer: B**

**175. Expression giving absolute difference between two dates?**  
A. $dateDiff  
B. $subtract  
C. $duration  
D. $minus  
**Answer: B**

**176. What happens if you shard populated collection without index on shard key?**  
A. Works automatically  
B. MongoDB auto-creates index  
C. Command fails  
D. Collection deleted  
**Answer: C**

**177. Jumbo chunk is:**  
A. Empty chunk  
B. Oversized chunk that cannot split  
C. Backup chunk  
D. Config server chunk  
**Answer: B**

**178. In a 3-shard cluster, how many replica sets?**  
A. 1  
B. 3  
C. 6  
D. 9  
**Answer: B**

**179. Command to see aggregation execution plan?**  
A. explain().aggregate  
B. aggregate with { explain:true }  
C. showPlan  
D. sh.status  
**Answer: B**

**180. Can a collection have more than one text index?**  
A. Yes, unlimited  
B. No, only one  
C. Yes, up to 3  
D. Yes, on different fields  
**Answer: B**

### **Unit 5: Node.js Integration (MCQs)**

**181. Which Node.js method converts a string ID into a MongoDB ObjectId?**  
A. ObjectId("64a...")  
B. String("64a...")  
C. MongoID("64a...")  
D. ToId("64a...")  
**Answer: A**

**182. In Node.js, `collection.find({})` returns:**  
A. An array  
B. A Promise of documents  
C. A Cursor  
D. A single document  
**Answer: C**

**183. Command to insert multiple docs in Node.js:**  
A. addMany  
B. insertArray  
C. insertMany  
D. saveMany  
**Answer: C**

**184. In a Replica Set, which node accepts writes?**  
A. Secondary  
B. Arbiter  
C. Hidden  
D. Primary  
**Answer: D**

**185. Correct way to connect using MongoClient:**  
A. MongoClient.connect(url)  
B. mongodb.open(url)  
C. db.connect(url)  
D. new Connection(url)  
**Answer: A**

**186. Aggregation stage that deconstructs arrays:**  
A. $group  
B. $unwind  
C. $project  
D. $split  
**Answer: B**

**187. Convert cursor to array in Node.js:**  
A. cursor.toList()  
B. cursor.toArray()  
C. cursor.fetch()  
D. cursor.json()  
**Answer: B**

**188. Best DB for social network relationships:**  
A. Document Store  
B. Column Family  
C. Graph DB  
D. Key-Value Store  
**Answer: C**

**189. Parent entry point of MongoDB Node.js driver:**  
A. Database  
B. Collection  
C. MongoClient  
D. Admin  
**Answer: C**

**190. In `insertOne`, where is the new document's ID stored?**  
A. newId  
B. insertedId  
C. _id  
D. documentId  
**Answer: B**

**191. Auto-created index in MongoDB collections:**  
A. name  
B. email  
C. created_at  
D. _id  
**Answer: D**

**192. Operator used to update a specific field without replacing whole document:**  
A. $replace  
B. $set  
C. $overwrite  
D. $modify  
**Answer: B**

**193. MongoDB stores data in which format?**  
A. JSON  
B. BSON  
C. XML  
D. YAML  
**Answer: B**

**194. Method to close active DB connection in Node.js:**  
A. client.stop()  
B. client.exit()  
C. client.close()  
D. client.disconnect()  
**Answer: C**

**195. Ideal use case for a Key-Value store like Redis:**  
A. Complex joins  
B. Billing ledger  
C. Session caching  
D. Spatial queries  
**Answer: C**

**196. What happens if you insert into a non-existent collection?**  
A. Error  
B. Collection auto-created  
C. DB crashes  
D. Document discarded  
**Answer: B**

**197. `collection.findOne({ name: "John" })` returns:**  
A. A cursor  
B. A Promise resolving to the document or null  
C. A synchronous document  
D. An array with one document  
**Answer: B**

**198. Index required for spherical geospatial queries:**  
A. 2d  
B. geoHaystack  
C. 2dsphere  
D. text  
**Answer: C**

**199. Default MongoDB TCP port:**  
A. 3306  
B. 5432  
C. 27017  
D. 8080  
**Answer: C**

**200. Feature introduced in MongoDB 4.0 enabling ACID across multiple documents:**  
A. Sharding  
B. Replication  
C. Multi-document Transactions  
D. Aggregation Framework  
**Answer: C**

### **Unit 6: Graph Databases (MCQs)**

**201. Which best describes the Labeled Property Graph model used by Neo4j?**  
A. Data stored as Subject–Predicate–Object triples  
B. Nodes and Relationships both store key-value properties  
C. Relationships inferred via foreign keys  
D. Data stored in columnar format  
**Answer: B**

**202. In Graph vs Relational DBs, what is equivalent to a Row?**  
A. Label  
B. Relationship  
C. Node  
D. Property  
**Answer: C**

**203. Primary characteristic of a Relationship in Neo4j:**  
A. Undirected and connects multiple nodes  
B. Always directed and must have a type  
C. Cannot store properties  
D. Represents an entity  
**Answer: B**

**204. Query language used by Neo4j:**  
A. SQL  
B. Gremlin  
C. SPARQL  
D. Cypher  
**Answer: D**

**205. Difference between `CREATE` and `MERGE` in Cypher:**  
A. CREATE is idempotent  
B. MERGE deletes existing data  
C. CREATE always adds new data; MERGE matches or creates  
D. They are synonyms  
**Answer: C**

**206. What happens when deleting a node with active relationships?**  
A. Node deleted, relationships remain  
B. DB auto-deletes relationships  
C. Query fails unless `DETACH DELETE` used  
D. Node archived  
**Answer: C**

**207. NOT an ideal use case for Graph DBs:**  
A. Social networks  
B. Fraud detection  
C. Simple flat data with heavy aggregations  
D. Route planning  
**Answer: C**

**208. How is data represented in RDF?**  
A. Key-value pairs  
B. Triples: Subject, Predicate, Object  
C. Nodes with properties only  
D. Tables with schemas  
**Answer: B**

**209. Keyword to update properties in Cypher:**  
A. UPDATE  
B. ADD  
C. SET  
D. INSERT  
**Answer: C**

**210. What does the Instance Model represent?**  
A. Whiteboard sketch  
B. Abstract schema  
C. Actual stored data  
D. Hardware configuration  
**Answer: C**

**211. Correct syntax for a relationship in Cypher:**  
A. (Node1)--(Node2)  
B. (Node1)-[:TYPE]->(Node2)  
C. [Node1] -> [Node2]  
D. {Node1} JOIN {Node2}  
**Answer: B**

**212. Traversal exploring layer-by-layer:**  
A. DFS  
B. BFS  
C. A\*  
D. Random Walk  
**Answer: B**

**213. How does graph-based fraud detection improve traditional methods?**  
A. Analyzing average transaction value  
B. Detecting repeated interaction patterns even with changing identifiers  
C. Using faster hardware for joins  
D. Enforcing FK constraints  
**Answer: B**

**214. What categorizes nodes in Neo4j (e.g., Person, Company)?**  
A. Properties  
B. Relationships  
C. Labels  
D. Indexes  
**Answer: C**

**215. What does `REMOVE` do in Cypher?**  
A. Deletes node & relationships  
B. Removes a label or property  
C. Disconnects relationship  
D. Drops database  
**Answer: B**

**216. Correct Cypher query to find all Person nodes named Ankit:**  
A. SELECT * FROM Person WHERE name='Ankit'  
B. MATCH (p:Person {name:'Ankit'}) RETURN p  
C. FIND (p:Person) WITH name 'Ankit'  
D. GET (p:Person) WHERE p.name=='Ankit'  
**Answer: B**

**217. True statement about schema in Graph DBs:**  
A. Requires rigid schema  
B. RDBMS allows flexible schema without migrations  
C. Graph DBs are schema-optional and flexible  
D. Both require same schema  
**Answer: C**

**218. Best relationship type for Student → Course:**  
A. :IS_A  
B. :ENROLLED_IN  
C. :CONTAINS  
D. :HAS_PROPERTY  
**Answer: B**

**219. What is a Cycle in graph theory?**  
A. Undirected relationship  
B. Path starting and ending at same node  
C. Node with no relationships  
D. Deleting database  
**Answer: B**

**220. Clause used with MATCH to filter by range:**  
A. FILTER  
B. HAVING  
C. WHERE  
D. WHEN  
**Answer: C**
### **Unit 6: Graph Databases (MCQs)**

**201. Which best describes the Labeled Property Graph model used by Neo4j?**  
A. Data stored as Subject–Predicate–Object triples  
B. Nodes and Relationships both store key-value properties  
C. Relationships inferred via foreign keys  
D. Data stored in columnar format  
**Answer: B**

**202. In Graph vs Relational DBs, what is equivalent to a Row?**  
A. Label  
B. Relationship  
C. Node  
D. Property  
**Answer: C**

**203. Primary characteristic of a Relationship in Neo4j:**  
A. Undirected and connects multiple nodes  
B. Always directed and must have a type  
C. Cannot store properties  
D. Represents an entity  
**Answer: B**

**204. Query language used by Neo4j:**  
A. SQL  
B. Gremlin  
C. SPARQL  
D. Cypher  
**Answer: D**

**205. Difference between `CREATE` and `MERGE` in Cypher:**  
A. CREATE is idempotent  
B. MERGE deletes existing data  
C. CREATE always adds new data; MERGE matches or creates  
D. They are synonyms  
**Answer: C**

**206. What happens when deleting a node with active relationships?**  
A. Node deleted, relationships remain  
B. DB auto-deletes relationships  
C. Query fails unless `DETACH DELETE` used  
D. Node archived  
**Answer: C**

**207. NOT an ideal use case for Graph DBs:**  
A. Social networks  
B. Fraud detection  
C. Simple flat data with heavy aggregations  
D. Route planning  
**Answer: C**

**208. How is data represented in RDF?**  
A. Key-value pairs  
B. Triples: Subject, Predicate, Object  
C. Nodes with properties only  
D. Tables with schemas  
**Answer: B**

**209. Keyword to update properties in Cypher:**  
A. UPDATE  
B. ADD  
C. SET  
D. INSERT  
**Answer: C**

**210. What does the Instance Model represent?**  
A. Whiteboard sketch  
B. Abstract schema  
C. Actual stored data  
D. Hardware configuration  
**Answer: C**

**211. Correct syntax for a relationship in Cypher:**  
A. (Node1)--(Node2)  
B. (Node1)-[:TYPE]->(Node2)  
C. [Node1] -> [Node2]  
D. {Node1} JOIN {Node2}  
**Answer: B**

**212. Traversal exploring layer-by-layer:**  
A. DFS  
B. BFS  
C. A\*  
D. Random Walk  
**Answer: B**

**213. How does graph-based fraud detection improve traditional methods?**  
A. Analyzing average transaction value  
B. Detecting repeated interaction patterns even with changing identifiers  
C. Using faster hardware for joins  
D. Enforcing FK constraints  
**Answer: B**

**214. What categorizes nodes in Neo4j (e.g., Person, Company)?**  
A. Properties  
B. Relationships  
C. Labels  
D. Indexes  
**Answer: C**

**215. What does `REMOVE` do in Cypher?**  
A. Deletes node & relationships  
B. Removes a label or property  
C. Disconnects relationship  
D. Drops database  
**Answer: B**

**216. Correct Cypher query to find all Person nodes named Ankit:**  
A. SELECT * FROM Person WHERE name='Ankit'  
B. MATCH (p:Person {name:'Ankit'}) RETURN p  
C. FIND (p:Person) WITH name 'Ankit'  
D. GET (p:Person) WHERE p.name=='Ankit'  
**Answer: B**

**217. True statement about schema in Graph DBs:**  
A. Requires rigid schema  
B. RDBMS allows flexible schema without migrations  
C. Graph DBs are schema-optional and flexible  
D. Both require same schema  
**Answer: C**

**218. Best relationship type for Student → Course:**  
A. :IS_A  
B. :ENROLLED_IN  
C. :CONTAINS  
D. :HAS_PROPERTY  
**Answer: B**

**219. What is a Cycle in graph theory?**  
A. Undirected relationship  
B. Path starting and ending at same node  
C. Node with no relationships  
D. Deleting database  
**Answer: B**

**220. Clause used with MATCH to filter by range:**  
A. FILTER  
B. HAVING  
C. WHERE  
D. WHEN  
**Answer: C**

### **Unit 6: Advanced Graph Database MCQs (Medium–Hard)**

**221. In the Property Graph Model, which is strictly true about properties?**  
A. Properties only on Nodes  
B. Properties limited to strings  
C. Properties are key-value pairs stored on both Nodes and Relationships  
D. Relationships can store properties only if undirected  
**Answer: C**

**222. To retrieve a node if it exists or create it if not, and set `createdAt` only on creation, you use:**  
A. CREATE + IF NOT EXISTS  
B. MERGE + ON CREATE SET  
C. MATCH + CREATE  
D. MERGE + ON MATCH SET  
**Answer: B**

**223. Why does `MATCH (p:Person)-[:WORKS_AT]->(c:Company) DELETE p` fail?**  
A. Cannot delete node with existing relationships  
B. DELETE must be at start  
C. Company must be deleted first  
D. Cypher cannot delete matched variables  
**Answer: A**

**224. Least suitable scenario for Graph DB:**  
A. Real-time recommendations  
B. IAM systems  
C. Massive linear transaction logs  
D. Fraud detection  
**Answer: C**

**225. Find employees whose name starts with 'R':**  
A. WHERE name LIKE 'R%'  
B. WHERE e.name STARTS WITH 'R'  
C. WHERE e.name BEGINS 'R'  
D. FILTER e.name = 'R*'  
**Answer: B**

**226. Best practice to model time-varying relationships (e.g., WORKS_AT 2010–2015):**  
A. New node per year  
B. Add start_date and end_date to relationship  
C. Create STARTED_AT and ENDED_AT relationships  
D. Store dates in Person node  
**Answer: B**

**227. Traversal performance advantage of Graph DBs:**  
A. SQL faster due to FKs  
B. Graph faster due to index-free adjacency  
C. Both equal  
D. Graph slower  
**Answer: B**

**228. Role of OPTIONAL MATCH:**  
A. Returns pattern if found, else null  
B. Forces index usage  
C. Matches only unconnected nodes  
D. Deletes relationship if matched  
**Answer: A**

**229. RDF triple components:**  
A. Node, Edge, Property  
B. Key, Value, Document  
C. Subject, Predicate, Object  
D. Row, Column, Family  
**Answer: C**

**230. Core assumption for graph-based fraud detection:**  
A. Fraudsters keep same credit cards  
B. Fraudsters change IDs, but interaction patterns repeat  
C. SQL needed for fraud  
D. Requires flat CSV files  
**Answer: B**

**231. What does `MATCH (n) DETACH DELETE n` do?**  
A. Deletes only nodes without relationships  
B. Deletes relationships only  
C. Deletes entire graph  
D. Creates backup  
**Answer: C**

**232. Correct statement about Neo4j schema:**  
A. Must define schema beforehand  
B. Neo4j cannot enforce constraints  
C. Schema-optional; properties flexible  
D. Changing type requires restart  
**Answer: C**

**233. Remove property `age` from node `p`:**  
A. DELETE p.age  
B. DROP p.age  
C. REMOVE p.age  
D. ALTER NODE p DROP age  
**Answer: C**

**234. Traversal exploring deepest branch first:**  
A. BFS  
B. DFS  
C. Shortest Path  
D. PageRank  
**Answer: B**

**235. Best model for tracking which semester a course was held:**  
A. Add semester to Student  
B. Course -[:HELD_IN]-> Semester  
C. Table for Semesters  
D. Add :Semester label to Course  
**Answer: B**

**236. SQL vs Graph complexity for mentor traversal:**  
A. SQL needs joins; Graph uses hops  
B. SQL needs hops; Graph uses joins  
C. SQL cannot model this  
D. Graph slower  
**Answer: A**

**237. NOT a valid Property Graph component:**  
A. Nodes  
B. Foreign Keys  
C. Relationships  
D. Labels  
**Answer: B**

**238. Name matched by `STARTS WITH 'M'`:**  
A. Sam  
B. McKenna  
C. Tom  
D. Ammy  
**Answer: B**

**239. Where should the Grade go in Student–Course model?**  
A. Student node  
B. Course node  
C. On :COMPLETED relationship  
D. On University node  
**Answer: C**

**240. Imperative graph query language:**  
A. Cypher  
B. SQL  
C. Gremlin  
D. GraphQL  
**Answer: C**

**241. Result of:**  
`MERGE (p:Person {name:'Naveen'}) ON MATCH SET p.lastLogin = timestamp()`  
A. Always creates new node  
B. Updates lastLogin if exists; creates node if not (without lastLogin)  
C. Errors if missing  
D. Deletes and recreates node  
**Answer: B**

**242. Why Graph DBs excel at Social Networks?**  
A. Fast simple key lookups  
B. Optimized for connected data traversal  
C. Rigid schema  
D. Store binary files  
**Answer: B**

**243. NoSQL type optimized for analytical queries:**  
A. Key-Value  
B. Document  
C. Column Family  
D. Graph  
**Answer: C**

**244. Relationship direction in Neo4j:**  
A. Must specify exact direction  
B. Can traverse either or ignore direction  
C. Only start→end allowed  
D. Becomes undirected  
**Answer: B**

**245. Graph data modeling includes:**  
A. Normalizing tables  
B. Designing node-relationship schema  
C. Defining PK/FK pairs  
D. Flattening to JSON  
**Answer: B**

**246. Valid relationship pattern:**  
A. (Person)-[WORKS_AT]-(Company)  
B. (Person)-[:WORKS_AT]->(Company)  
C. (Person) -> (Company)  
D. JOIN syntax  
**Answer: B**

**247. A cycle represents:**  
A. Infinite path  
B. Path starting & ending same node  
C. Relationship with no props  
D. Node without edges  
**Answer: B**

**248. List all property keys:**  
A. SHOW TABLES  
B. CALL db.propertyKeys()  
C. DESCRIBE GRAPH  
D. SELECT keys  
**Answer: B**

**249. Weighted relationships are used for:**  
A. Password storage  
B. Route planning cost/distance  
C. Label indexing  
D. PK definition  
**Answer: B**

**250. Query to find classmates:**  
A. Find all courses then students  
B. Student → ENROLLED_IN → Course ← ENROLLED_IN ← Students  
C. SQL course_id join  
D. Scan all Student nodes  
**Answer: B**

**251. Why MERGE is idempotent?**  
A. Always errors  
B. Re-running yields same state; no duplicates  
C. Deletes before writing  
D. Creates duplicates  
**Answer: B**

**252. Meaning of (e:Employee):**  
A. Property e = Employee  
B. Relationship type Employee  
C. Node with label Employee, variable e  
D. Property named Employee  
**Answer: C**

**253. How Neo4j stores null properties:**  
A. Special NULL marker  
B. Empty string  
C. Property omitted entirely  
D. Stores 0  
**Answer: C**

**254. Limitation of Graph DBs:**  
A. Cannot handle social graphs  
B. Not ideal for heavy aggregations  
C. Cannot store text  
D. Slower for simple lookups  
**Answer: B**

**255. Cypher to find 'Ankit' and return designation:**  
A. MATCH (p:Person {name:'Ankit'}) RETURN p.designation  
B. SQL equivalent  
C. RETURN with FROM clause  
D. FIND syntax  
**Answer: A**

**256. Data Model is analogous to:**  
A. Table rows  
B. Schema blueprint  
C. Memory address  
D. Log file  
**Answer: B**

**257. Clause to update multiple properties:**  
A. UPDATE  
B. SET n.p1=..., n.p2=...  
C. MODIFY  
D. CHANGE  
**Answer: B**

**258. In telecom fraud graph, what is a Node?**  
A. Call duration  
B. Subscriber/phone number  
C. CALLED relationship  
D. Timestamp  
**Answer: B**

**259. Filter relationship properties by range:**  
A. Inside [] brackets  
B. RETURN clause  
C. WHERE clause  
D. Impossible  
**Answer: C**

**260. NOT a graph benefit:**  
A. Flexible schema-less structure  
B. Relationships first-class  
C. Native SQL JOIN support  
D. Fast traversal  
**Answer: C**

### **Unit: Storage Engines, GridFS, Security, Encryption & Auditing (MCQs)**

**261. Which storage engine is the default for MongoDB?**  
A. MMAPv1  
B. WiredTiger  
C. In-Memory  
D. Encrypted Storage Engine  
**Answer: B**

**262. WiredTiger provides which level of concurrency?**  
A. Database-level  
B. Collection-level  
C. Document-level  
D. Field-level  
**Answer: C**

**263. Maximum size of a single MongoDB journal file:**  
A. 64 MB  
B. 100 MB  
C. 256 MB  
D. 1 GB  
**Answer: B**

**264. What happens to In-Memory storage engine data if server crashes?**  
A. Recovered from journal  
B. Recovered from oplog  
C. Saved to disk before crash  
D. Lost completely (rollback occurs)  
**Answer: D**

**265. Default compression algorithm in WiredTiger:**  
A. zlib  
B. LZ4  
C. Snappy  
D. Gzip  
**Answer: C**

**266. Primary purpose of journaling:**  
A. Replication  
B. Durability & crash recovery  
C. Data compression  
D. Data encryption  
**Answer: B**

**267. In hybrid replica sets, In-Memory nodes are used for:**  
A. Historical logs  
B. High-latency writes  
C. Ultra-low latency queries  
D. Reducing cost  
**Answer: C**

**268. TRUE statement about Journaling vs Oplog:**  
A. Oplog on local FS, journaling is a collection  
B. Journaling for replication, oplog for crash recovery  
C. Journal files are long-lived, oplog short-lived  
D. Journaling logs physical changes; oplog logs logical ops  
**Answer: D**

**269. Feature that creates snapshots for crash consistency:**  
A. Sharding  
B. Journaling  
C. Checkpointing  
D. GridFS  
**Answer: C**

**270. WiredTiger Enterprise Edition adds:**  
A. Document-level concurrency  
B. Encryption at Rest  
C. Journaling  
D. Indexing  
**Answer: B**

---

### **Unit: GridFS**

**271. Default GridFS chunk size:**  
A. 16 MB  
B. 100 MB  
C. 255 KB  
D. 64 KB  
**Answer: C**

**272. Collections created automatically by GridFS:**  
A. fs.data & fs.metadata  
B. fs.files & fs.chunks  
C. grid.files & grid.blocks  
D. fs.master & fs.detail  
**Answer: B**

**273. GridFS is used for files larger than:**  
A. 4 MB  
B. 8 MB  
C. 16 MB  
D. 32 MB  
**Answer: C**

**274. Limitation of GridFS:**  
A. Max file size 1 GB  
B. No atomic writes for large files  
C. Enterprise only  
D. Needs separate process  
**Answer: B**

**275. Command to upload file with mongofiles:**  
A. mongofiles insert  
B. mongofiles upload  
C. mongofiles put  
D. mongofiles push  
**Answer: C**

---

### **Unit: Security, Authentication & Authorization**

**276. Config setting to enable authorization:**  
A. security.authentication: enabled  
B. security.authorization: enabled  
C. system.security: active  
D. access.control: on  
**Answer: B**

**277. Role allowing user creation/modification across all DBs:**  
A. dbAdmin  
B. readWriteAnyDatabase  
C. userAdminAnyDatabase  
D. clusterAdmin  
**Answer: C**

**278. Principle of Least Privilege:**  
A. All users should be admins  
B. Users get only required permissions  
C. Only root needs password  
D. Disable authorization for speed  
**Answer: B**

**279. Default IP MongoDB binds to:**  
A. 0.0.0.0  
B. 192.168.1.1  
C. 127.0.0.1  
D. None  
**Answer: C**

**280. Section to modify for external connections (`bindIp`):**  
A. systemLog  
B. storage  
C. net  
D. processManagement  
**Answer: C**

---

### **Unit: Encryption & Auditing**

**281. Technology for encrypting traffic (data in transit):**  
A. SSH  
B. TLS/SSL  
C. WPA2  
D. MD5  
**Answer: B**

**282. Client-Side Field Level Encryption ensures:**  
A. Server encrypts after receiving  
B. Encryption happens before leaving client; server stores ciphertext only  
C. Full DB encrypted by OS  
D. Only admins can view data  
**Answer: B**

**283. Algorithm used for data-at-rest encryption:**  
A. DES  
B. AES-256  
C. RSA-2048  
D. SHA-256  
**Answer: B**

**284. NOT a valid audit log target:**  
A. Console  
B. Syslog  
C. HTML file  
D. JSON file  
**Answer: C**

**285. Requirement for audit logs to maintain total order:**  
A. DB must be sharded  
B. Journaling must be enabled  
C. Log format must be BSON  
D. Must run on Linux  
**Answer: B**

**286. Command to create a user:**  
A. db.addUser()  
B. db.createProfile()  
C. db.createUser()  
D. db.insertUser()  
**Answer: C**

**287. readWrite role allows:**  
A. Only read  
B. Read + modify data in DB  
C. Modify roles  
D. Cluster admin tasks  
**Answer: B**

**288. Where does decryption occur in CSFLE?**  
A. Server  
B. Load balancer  
C. Client-side only  
D. Backup server  
**Answer: C**

**289. Prevents MITM attacks:**  
A. Journaling  
B. TLS/SSL  
C. Compression  
D. GridFS  
**Answer: B**

**290. What does `fs.files` store?**  
A. File binary content  
B. File metadata  
C. User auth logs  
D. Server config  
**Answer: B**
### **Firebase MCQs (Setup, CLI, Config, SDK) — Numbering Continues**

**291. What is the name of the free Firebase pricing plan?**  
A. Blaze  
B. Flame  
C. Spark  
D. Ember  
**Answer: C**

**292. When creating a Firebase project, what unique identifier is auto-generated?**  
A. Project Key  
B. Project ID  
C. Project Secret  
D. Project Hash  
**Answer: B**

**293. Which service is highlighted in the "Build" sidebar in the screenshots?**  
A. Crashlytics  
B. Authentication  
C. Performance Monitoring  
D. Test Lab  
**Answer: B**

**294. First step to get started in Firebase Console:**  
A. Create a database  
B. Create a new Firebase project  
C. Install the CLI  
D. Write Cloud Functions  
**Answer: B**

**295. The `firebaseConfig` object is written in which format?**  
A. XML  
B. YAML  
C. JSON / JavaScript Object  
D. SQL  
**Answer: C**

---

### **Installation & CLI**

**296. Command to install Firebase CLI globally:**  
A. npm install firebase  
B. npm install -g firebase-tools  
C. npm start firebase  
D. npm download firebase-cli  
**Answer: B**

**297. Difference between `firebase` and `firebase-tools` packages:**  
A. Same package  
B. `firebase` = client SDK; `firebase-tools` = CLI  
C. `firebase` = server; `firebase-tools` = client  
D. `firebase-tools` is deprecated  
**Answer: B**

**298. Command to authenticate CLI with Google account:**  
A. firebase signin  
B. firebase auth  
C. firebase login  
D. firebase connect  
**Answer: C**

**299. Flag to list all Firebase CLI commands:**  
A. firebase --list  
B. firebase --all  
C. firebase --help  
D. firebase --status  
**Answer: C**

**300. General syntax of Firebase CLI commands:**  
A. firebase [arguments] <command> [option]  
B. firebase <command> [option] [arguments]  
C. <command> firebase [option]  
D. npm firebase <command>  
**Answer: B**

**301. CLI command used for creating a project:**  
A. firebase projects:new  
B. firebase projects:create  
C. firebase create:project  
D. firebase init  
**Answer: B**

**302. npm prerequisite implies installation of:**  
A. Python  
B. Java  
C. Node.js  
D. Docker  
**Answer: C**

---

### **firebaseConfig Object**

**303. Field identifying the project on Google servers:**  
A. clientSecret  
B. apiKey  
C. adminKey  
D. privateId  
**Answer: B**

**304. Purpose of `authDomain`:**  
A. Stores user passwords  
B. Domain used for OAuth redirects  
C. URL of database  
D. Hosting URL for images  
**Answer: B**

**305. Field associated with Firebase Storage:**  
A. storageBucket  
B. databaseURL  
C. assetPath  
D. fileStore  
**Answer: A**

**306. Field specifically related to Google Analytics:**  
A. projectId  
B. authDomain  
C. measurementId  
D. storageBucket  
**Answer: C**

**307. For which SDK versions is `measurementId` optional?**  
A. All versions  
B. v7.20.0 and later  
C. v9.0.0 only  
D. Never optional  
**Answer: B**

**308. Likely authDomain for projectId = "demopject-af2cf":**  
A. demopject-af2cf.google.com  
B. demopject-af2cf.firebaseapp.com  
C. demopject-af2cf.web.app  
D. auth.demopject-af2cf.com  
**Answer: B**

---

### **SDK & Code Implementation**

**309. Import syntax for Firebase Modular SDK (v9+):**  
A. require('firebase')  
B. import firebase from "firebase/app"  
C. import { initializeApp } from "firebase/app"  
D. include "firebase.js"  
**Answer: C**

**310. First function called to initialize Firebase:**  
A. startFirebase()  
B. createApp()  
C. initializeApp()  
D. getApp()  
**Answer: C**

**311. Required argument for `initializeApp`:**  
A. Project name  
B. firebaseConfig object  
C. User email  
D. API key only  
**Answer: B**

**312. Function imported to use Analytics:**  
A. startAnalytics  
B. getAnalytics  
C. initAnalytics  
D. logEvent  
**Answer: B**

**313. Argument passed to `getAnalytics`:**  
A. firebaseConfig  
B. app instance  
C. apiKey  
D. Nothing  
**Answer: B**

**314. Import path for `initializeApp`:**  
A. firebase/init  
B. firebase/core  
C. firebase/app  
D. firebase/utils  
**Answer: C**

**315. Where to find list of available web SDK libraries:**  
A. package.json  
B. node_modules  
C. firebase.google.com/docs/web/setup#available-libraries  
D. firebaseConfig object  
**Answer: C**

---

### **Deep & Conceptual**

**316. Why use `npm install firebase` (without -g)?**  
A. Install CLI tools  
B. Add Firebase SDK to project dependencies  
C. Create new cloud project  
D. Login to console  
**Answer: B**

**317. Meaning of `// Need to Delete` in provided code:**  
A. Mandatory line  
B. Placeholder/template to be removed  
C. API Key reference  
D. Analytics import  
**Answer: B**

**318. storageBucket for projectId = "demopject-af2cf":**  
A. demopject-af2cf.com  
B. demopject-af2cf.firebasestorage.app  
C. demopject-af2cf.storage.googleapis.com  
D. demopject-af2cf.s3.amazonaws.com  
**Answer: B**

**319. NOT a valid firebaseConfig key:**  
A. apiKey  
B. databaseSecret  
C. authDomain  
D. projectId  
**Answer: B**

**320. What indicates Analytics initialized successfully?**  
A. firebaseConfig object exists  
B. analytics = getAnalytics(app) is assigned  
C. User logs in via CLI  
D. Console logs "Hello, ankit"  
**Answer: B**
