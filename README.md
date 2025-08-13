The program - GEO POINTS DATABASE - changes the [MlengelaPD8](https://github.com/CIS1250Python/MlengelaPD8/blob/main/MlengelaDP8.zip) so that instead of reading in a list of five or more points from a file, the project will read the points in from a database.
Here's what the program does: 
1. The created program creates a database and inserts at least five points. The following are the points to be used:
    * 35.0714,106.6289, Main Campus
    * 35.0998,104.0639, Montoya
    * 35.2328,106.6630, Rio Rancho
    * 35.0856,106.6493, STEMULUS Center
    * 35.1836,106.5939, ATC
2. Run the database to initialize the code to create the database.
3. Modify the GUI program from [MlengelaPD10](https://github.com/CIS1250Python/MlengelaPD10/blob/main/MlengelaDP10.zip) so that it reads points from my database instead of a file.
## Basic Process: 
The Program manipulates the database with the following applications: 
1. SQLite3 Library, which is included with my Python installation. A programmer can also pipping install it whenever necessary.
   * import sqlite3
2. There must be a connection to a database to be able to write to it.
   * conn=sqlite3.connect('Mlengeladabase.db')
3. If 'Mlengeladabase.db' does not exist, then it will create it.
4. 'Mlengeladabase.db' will then appear in the same directory as the program (Unless you provide a path, then it will appear there instead)
5. A cursor must be used to execute SQL queries
   * curs=conn.cursor()
6. Once all changes are done, you must commit them to the database
   * conn.commit()
   * You can and should commit each time you've modified the database, not just when you're ready to close it.
7. When you no longer need access to the database, use the close method to close it.
   * conn.close()
   * This is important when multiple users are using the database, since most databases can only support a limited number of simultaneous connections.

## Structured Query Language (SQL)
  * Language designed to provide commands to databases.
  * Provides capabilities to:
      * Create rows of data in tables
      * Read data from tables
      * Update data in tables
      * Delete data from tables
  * CRUD is a common acronym to refer to data functions
  * SQL also provides you the capability to Create and Delete tables from databases.
  * In SQLite, table rows normally have a 64-bit signed integer ROWID, which is unique among all rows in the same table.
  * WITHOUT ROWID addition to tables is the exception.
  * Execute SQL statements on a database
  * Pass a SQL command to the cursor.execute method as a string:
      * curs.execute('..SQL command...')
## Create a table
<img width="1121" height="664" alt="image" src="https://github.com/user-attachments/assets/7e7459d6-f582-414f-93dc-ebb854611de6" />

## The program appears like this: 
<img width="1244" height="649" alt="image" src="https://github.com/user-attachments/assets/55e6214d-026d-4d45-aaca-923a55d17a47" />

## SQL CREATE TABLE
<img width="728" height="295" alt="image" src="https://github.com/user-attachments/assets/6d969586-7440-4dff-8280-edf2c99a64bd" />

## SQL INSERT INTO
<img width="1238" height="673" alt="image" src="https://github.com/user-attachments/assets/56f2ce61-65d9-4c93-a394-24e11017c841" />

##SQL UPDATE
<img width="1238" height="600" alt="image" src="https://github.com/user-attachments/assets/418132df-86b7-4663-829a-750e8cfb1e13" />

##SQL DELETE
<img width="1238" height="566" alt="image" src="https://github.com/user-attachments/assets/e2a30736-7b83-457e-bcd3-19b185d52d11" />

## Delete the existing database, then add some code to insert some starting data
<img width="1122" height="663" alt="image" src="https://github.com/user-attachments/assets/5edc6473-0672-4348-ae2f-2b559ad88967" />

## Initialize a Set of Data
<img width="941" height="708" alt="image" src="https://github.com/user-attachments/assets/e42e8d78-8c58-4714-825c-60abd8f1513b" />

## Create a program that performs Create, Read, Update, and Delete functions on the database. 
## fetchall()
<img width="1244" height="624" alt="image" src="https://github.com/user-attachments/assets/7ff08882-2a60-4860-a589-33cf83de4b4d" />

## As the program runs: 
<img width="1244" height="511" alt="image" src="https://github.com/user-attachments/assets/c721677d-7889-42c4-a598-2789822787be" />

## Display one record
<img width="1244" height="625" alt="image" src="https://github.com/user-attachments/assets/b6961237-b65d-4f50-ba5d-d9b748a600b2" />

## As it runs: 
<img width="1244" height="502" alt="image" src="https://github.com/user-attachments/assets/a64da181-61b3-4721-98f6-50f459033f37" />

##Formatting Output
<img width="1070" height="537" alt="image" src="https://github.com/user-attachments/assets/6831363d-8995-43e5-9e9d-3551b86aab21" />

<img width="1167" height="449" alt="image" src="https://github.com/user-attachments/assets/6bf90e7d-2fdd-4e16-b06c-5dde18eec672" />

## Insert Data
<img width="989" height="703" alt="image" src="https://github.com/user-attachments/assets/7de89fe9-4ab1-4ad5-a1ed-b80348a2dd2a" />

<img width="1086" height="650" alt="image" src="https://github.com/user-attachments/assets/a751f686-9620-4c89-bf9b-6e71e1cf08fa" />

## Update Data
<img width="1284" height="663" alt="image" src="https://github.com/user-attachments/assets/fa60abd5-b2e0-4984-94ef-b2651b198787" />

## Delete Data
<img width="1432" height="681" alt="image" src="https://github.com/user-attachments/assets/f6e0e9fa-2205-4ec9-8bf6-0c248134dbff" />

## Summary
   * Sqlite3
   * Connections
   * Commit
   * Close
   * Basic Process
   * SQL
   * Initializing a Database
   * CRUD



