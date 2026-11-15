# Database

> *A database is defined as an organized collection of related data stored systematically in a computer for convenient access.*

## Database Management System - DBMS

> *The system software that manages the database and provides tools to systematically create, retrieve and update the stored data is called a database management system.*

For example, MySQL, SQLite, Oracle Database.
## Database Model

> *A database model defines the logical design of the data and how seperate pieces of data relate to one another.*

1. **Heirarchical Model** -> Organizes data into a *tree* structure where each record has exactly one parent and may have multiple children. Older model, no longer used today.
2. **Network Model** -> Organizes data into a *graph* structure where records can have multiple parents and can be accessed by multiple paths. Older model, no longer used today.
3. **Relational Model** -> Organizes data into *tables* (2D, also called relations) that connect to eachother through shared values. Most commonly used in modern computing.

![Database Models|441](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Feud4ll0p512pxyghk2yl.png)

## Data Heirarchy

Data in a database is built layer by layer.
$$\text{Bit} \longrightarrow \text{Character} \longrightarrow \text{Field} \longrightarrow \text{Record} \longrightarrow \text{Table} \longrightarrow \text{Database}$$
+ Bit -> 1 or 0
+ Character -> Atleast 8 bits representing a single letter, symbol or number.
+ Field -> Group of characters holding a single piece of information.
+ Record -> Group of related fields describing a single entity.
+ Table -> Group of related record in a row and column format.
+ Database -> Collection of one or more tables managed together.

## Characteristic of a Good Database 

1. *Data Integrity* -> Stored data is valid, accurate and reliable.
2. *Data Independence* -> Data is seperate from software or logic.
3. *Avoids Data Redundancy* -> No data is repeated.
4. *Data Security* -> Only authorized users may access the data.
5. *Data Maintenance* -> Set procedures for manipulating data and optimizations.

## Relational Database Model

### Relations

> *A 2-dimensional table into which data is organized is formally known as a relation in a the relational database model.*

+ Each relation in a database must have a unique name.
+ Relations (tables) connect to eachother by sharing a common value.

### Attributes vs Tuples

+ **Attributes** refers to the column heading in a relational database. Every attribute in a relation must be unique.
	+ Number of attributes or columns in a table/relation is referred to as the *degree of the relation.*
	+ For example, in a `Students` relation; `Name`, `Roll Number` and `Gender` may be attributes.
+ **Tuples** refer to each row in a relational database which acts as a collection of attribute values that completely describe and entity.
	+ Number of tuples or rows (or basically, entries) in a table/relation is referred to as the *cardinality of the relation.*
	+ For example, `<L230844, Ahmed Muaz, Male>` may be a tuple in the `Students` relation.


>[!NOTE] Logical Design vs Physical Memory Layout
> Even if the data is logically designed as a table, it does not mean that the database is actually stored as a 2D table in memory but rather, the DBMS may choose any memory layout suitable for storing the database and will abstract over the layout with the logical design.

### Database Key

> *A database key is defined as an attribute or group of attributes whose values are guaranteed to uniquely identify a single record in a relation.*

#### Types of Keys

- **Candidate Key**:
	- A candidate key is an attribute or set of attributes that can uniquely identify a tuple. It is any column (or set of columns) that qualifies to be the main identifier.
	- _Example_: In an `Employee` table, `Employee_ID`, `SSN`, and `Passport_Number` are all Candidate Keys because each one individually can uniquely identify a person.
- **Primary Key (PK)**:
	- The **single Candidate Key** officially chosen by the database designer to uniquely identify each row.
	- _Rule_: A Primary Key **must be UNIQUE** and **cannot contain NULL (empty) values**[1][5].
- **Alternate Key**:
	- Any Candidate Key that was **not** chosen as the Primary Key.
	- _Example_: If `Employee_ID` is chosen as the Primary Key, then `SSN` and `Passport_Number` become Alternate Keys.
- **Super Key**:
	- Any combination of attributes that can uniquely identify a row.
	- _Example_: `Employee_ID` alone identifies an employee. Therefore, combining `(Employee_ID, Employee_Name)` is also a Super Key—even though adding the name is extra, the combination still uniquely identifies the row.
- **Foreign Key (FK)**:
	- A column in one table that links to the **Primary Key** of another table to connect the two tables together.
	- _Analogy_: In an `Attendance` table, storing the student's `RollNum` links that attendance record directly to the main `Student` table.
- **Composite Key (Concatenated Key)**:
	- A Primary Key made by combining **two or more columns** together when no single column is unique on its own.
	- _Example_: In a course enrollment table, combining `(Emp_ID, Proj_ID)` forms a Composite Key.
- **Artificial Key**:
	- A synthetic, auto-generated single column (like an auto-incremented `Row_Id` or serial number) added to a table when the natural primary key is too large or complex.