# Database Essentials & Relational Model

## 5-1 Understanding Data,Information (Organized Data) And Database

### What is DBMS?

- DBMS is database management system.
- A database is a structured Collection of Related Data that represents some real world entities and organized for efficient retrieval storage and management.
- If data are not related we can not tell them as database. If there is no relation between data we can not grab data doing queries. and the data will be real-world entities(physical, logical, Digital) like human,car or other.

#### Lets Breakdown More

- Database is nothing but computer. We can make our computer a database as well. The data will be stored in hard drive. And the data is retrieved and post using database management system (DBMS). Before hard disk or ssd data used to be stored in drum memory that looks like drum.

### What is Data?

- Data is facts that can be recorded in the form of .... (anything like:text,video,audio, speech form)

![alt text](<WhatsApp Image 2025-05-09 at 19.14.58_57fddcc3.jpg>)

- Data is Everywhere. we can access from any device and from anywhere. and all the data is stored in database.
- Data Is a crucial Thing, Chat Gpt has a huge collection of data nad thats why its growing faster.
- Data is the heart of digital World.

### What is Information?

- Information is processed and organized Data that provides meaningful context,insight or knowledge

![alt text](<WhatsApp Image 2025-05-09 at 20.35.02_9a8c43ba.jpg>)

## 5-2 What is DBMS and Why?

- Full Form Of DBMS is Database Management System. which manages data. In easy word DBMS is a piece of software by using we can manage our database.
- here is another thing named RDBMS- Which means relational database management system.

### Why DBMS IS Required?

- Why we need a database? we can store our data using our file system provided by our pc right? why should we install dbms software and use Database?

#### Lets Understand

![alt text](<WhatsApp Image 2025-05-09 at 21.34.01_a021322d.jpg>)

- Suppose we will use our file system to store the data, Open notepad and save in a file which will store in HDD or SSD.

##### What are the problems with it??

- `Unstructured data`, multiple formate (.txt,.mp4,etc) anything we can add or added by others. There will be no constrain. The data we are storing might have different extension like .mp4,.mp3.txt (means different type of data we save). To use the data we have to use different softwares to see each type of data. Based On The operating system the softwares are different as well. This is completely chaos. This is why unified data storage which is not possible in file system.
- `Data Redundancy` In case of sharing the data we have to make copies then send to our friends. This is causing data redundancy since we are making the copy of same data multiple time.

- `Data Inconsistency` While creating the data copy there anomaly is created means data inconsistency. Suppose we are making 10 duplicates and now we have to update a name it will be changed in my copy others will not be changed or we have to change manually.
- `No Concurrency Protocol` If everyone wants to access th data at a time there will be issue. There is not locking mechanism for read write. Its like one have to wait to do operation until previous one finished.
- `Security Issue` If we ant to access the file we want tyo access we must know the file path name exactly. There is a change of exposer of path. In file system either full file access should be given or nothing will be given no chance to show specific portion of the file.
- `Access Complication` If there is Millions of data and we want to search the data we have to search each and every data within Millions. But In DBMS data is stored in tabular format and each table is inter connected and the searching mechanism is implemented and it helps to find a data within a short time.

#### For All the Problems We Use Database Management System(DBMS).

- We are storing the data using file system but there will be a wrapper(DBMS Software). All the issues with te File systems are handled By DBMS.
- DBMS uses file system under the hood and the data will be stored in HDD or SSD.
- Suppose I want to store the data in database using DBMS. After storing the data i can use some unified commands in my DBMS to get the data delete the data post some other data and manage data. To do the communication We have to SQL(Structured Query Language)

![alt text](<WhatsApp Image 2025-05-09 at 22.07.24_1ab696f4.jpg>)

- SQL is a Query Language Its not a Programming language. SQL Gives us English Like Syntax by this we can instruct the DBMS and manage the data.
- So we have got a unified language to use the database in any system.

#### There Are Different Types Of Database

| Feature    | Description                           |
| ---------- | ------------------------------------- |
| Relational | MySQL, PostGreSQL, SQLite, SQL Server |
| Document   | MongoDB, DynamoDB                     |
| Key Value  | Redis                                 |

## 5-3 Different Type Of Database Model And Relational Model.

- There were different models of database.
  1. Hierarchical
  2. Network
  3. Relational
  4. Document
  5. Redis

### Hierarchical Model

- Hierarchical Model Used to Store data in Tree Structure.
  ![alt text](<WhatsApp Image 2025-05-10 at 09.48.15_175fa626.jpg>)
- If the data collection is vast it was difficult to visualize or finding data.
- Each Node Might have multiple children but one children must have one parent not more not less. This is a drawback.

### Network Model

- The problem of the Hierarchical Model is solved here, here we could share children within two parent node.
- ![alt text](<WhatsApp Image 2025-05-10 at 09.52.38_c176d720.jpg>)

- Complexity

  1. User had to navigate through a network of pointers to access or modify data,making it less intuitive than relational database.
  2. If data is vast we have to pass a lot of pointers if we want to search.

- Defining schema was very much

  1. Defining schema in network model could be more complex than relational data model.
  2. Schema Updating Was More complex as well.

- Lack Of Standardization
  1. There was no standardize Query Language.
  2. Different system or software were used to do query.
  3. Different Company Implemented Differently.

### Relational Model

- In Relational Model Data are stored separately
- The Separation is Done Using Table.

![alt text](<WhatsApp Image 2025-05-10 at 10.07.07_3147a00b.jpg>)

- First one Was Physical Entity and Second One was Hypothetical/Logical Entity.
- Using the Unique Key "u_id" or "o_id" we can identify a row.
- If there was no Unique Identifier we could not separate the duplicate data
- In Relational Database Linking data was done using unique Identifier.

![alt text](<WhatsApp Image 2025-05-10 at 10.14.19_3f4b7310.jpg>)

- u_id added in the product table, this helps to find out whose product is it. this type of referring key is named as foreign key.
- How The relation is created and how the relation is handled its pre defined. There will be some predefined rules which we will maintain and command. This will make relation between two data. DBMS takes the command and do the operation accordingly our command.

![alt text](<WhatsApp Image 2025-05-10 at 10.20.01_a64077a7.jpg>)

## 5-4 Anatomy Of a Table/Relation

![alt text](<WhatsApp Image 2025-05-10 at 10.47.10_42f7fa73.jpg>)

#### lets Breakdown The table

- Tables are called relation
- Before doing a project we have to define the entity first, like users can be one entity, the order they are placing this will be another entity. and the entities are represented by table.
- First we have to give a table name. suppose the user data is stored in user table.
- Columns of the table are called Column/Attribute. we can give a constrain/domain in the column, its like fixed domain data will be here like email column only the emails will be here.
- Its like fixed domain data of birth will be here like date column only the dates will be here.
- All The columns are called degree together (collection of columns)
- If we start to put the data in a row and accordingly the column. all the data are called Row/Tuple/Record. All the Rows are together called Rows/Records/Tuples or `Cardinality`.
- High Cardinality Means Many Rows and Low Cardinality Means Less Rows

![alt text](<WhatsApp Image 2025-05-10 at 11.04.22_05be4085.jpg>)
