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
