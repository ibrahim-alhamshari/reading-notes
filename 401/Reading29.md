## Save data in a local database using Room
- It's very good for the user, where it allows him to access the data when he ofline.

- In Android, there are 2 ways of providing offline storage of data:
    1. Room Database
    2. Preferences (SharedPreference and Preference DataStore).


![Room dataBase](https://developer.android.com/images/training/data-storage/room_architecture.png)

* There are three major components in Room:
    1. The database class
    2. Data entities that represent tables in the app's database.
    3. Data access objects (DAOs): It provides methods that the app can use to read, update, insert, and delete data in the database.

## Defining data using Room entities

- Entities: It represents the objects that we want to store in the database, and each instance of an entity represents a row of data in the corresponding table. So, we use it to define the schema.

- By default, Room uses the class name as the database table name. If you want the table to have a different name, set the tableName property of the @Entity annotation. Similarly, Room uses the field names as column names in the database by default. If you want a column to have a different name, add the @ColumnInfo annotation to the field and set the name property.

## Define relationships between objects
- We can specify relationships between entities and allow entity objects to reference each other.
1. Define one-to-one relationships
2. one-to-many relationship
3. many-to-many relationship
4. nested relationship

## Accessing data using Room DAOs
- DAO(data access object): It includes methods that offer abstract access to your app's database.

* There are two types of DAO methods that define database interactions:

* Convenience methods that let you insert, update and delete rows in your database without writing any SQL code.
* Query methods that let you write your own SQL query to interact with the database.

    * The `@Insert` annotation allows you to define methods that insert their parameters into the appropriate table in the database.
    * The `@Update` annotation allows you to define methods that update specific rows in a database table.
    * The `@Delete` annotation allows you to define methods that delete specific rows from a database table.
    * The @Query annotation allows you to write SQL statements and expose them as DAO methods.

### Resources
- https://developer.android.com/training/data-storage/room
- https://developer.android.com/training/data-storage/room/defining-data
- https://developer.android.com/training/data-storage/room/relationships
- https://developer.android.com/training/data-storage/room/accessing-data#java