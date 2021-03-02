
# DB Normalization

![images](images/Nor.jpg)

## What is Normalization?
- Normalization is a database design technique that reduces data redundancy and eliminates undesirable characteristics like Insertion, Update and Deletion Anomalies. Normalization rules divides larger tables into smaller tables and links them using relationships. The purpose of Normalization in SQL is to eliminate redundant (repetitive) data and ensure data is stored logically.

## Database Normal Forms
- Here is a list of Normal Forms

    1. 1NF (First Normal Form)
    2. 2NF (Second Normal Form)
    3. 3NF (Third Normal Form)
    4. BCNF (Boyce-Codd Normal Form)
    5. 4NF (Fourth Normal Form)
    6. 5NF (Fifth Normal Form)
    7. 6NF (Sixth Normal Form)

- normalization achieves its best in 3rd Normal Form

### 1NF (First Normal Form) Rules

- Each table cell should contain a single value.
- Each record needs to be unique.

### What is a KEY?
- A KEY is a value used to identify a record in a table uniquely. A KEY could be a single column or combination of multiple columns

#### What is a Primary Key?

- A primary is a single column value used to identify a database record uniquely.

- It has following attributes

    1. A primary key cannot be NULL
    2. A primary key value must be unique
    3. The primary key values should rarely be changed
    4. The primary key must be given a value when a new record is inserted.

### 2NF (Second Normal Form) Rules
- Rule 1- Be in 1NF
- Rule 2- Single Column Primary Key


### 3NF (Third Normal Form) Rules
- Rule 1- Be in 2NF
- Rule 2- Has no transitive functional dependencies

### BCNF (Boyce-Codd Normal Form)
- Even when a database is in 3rd Normal Form, still there would be anomalies resulted if it has more than one Candidate Key.

- Sometimes is BCNF is also referred as 3.5 Normal Form.

### 4NF (Fourth Normal Form) Rules
- If no database table instance contains two or more, independent and multivalued data describing the relevant entity, then it is in 4th Normal Form.

### 5NF (Fifth Normal Form) Rules
- A table is in 5th Normal Form only if it is in 4NF and it cannot be decomposed into any number of smaller tables without loss of data.

### 6NF (Sixth Normal Form) Proposed
- 6th Normal Form is not standardized, yet however, it is being discussed by database experts for some time. Hopefully, we would have a clear & standardized definition for 6th Normal Form in the near future...

That's all to SQL Normalization!!!

# Summary
- Database designing is critical to the successful implementation of a database management system that meets the data requirements of an enterprise system.
- Normalization Process in DBMS helps produce database systems that are cost-effective and have better security models.
- Functional dependencies are a very important component of the normalize data process
- Most database systems are normalized database up to the third normal forms.
- A primary key uniquely identifies are record in a Table and cannot be null
- A foreign key helps connect table and references a primary key