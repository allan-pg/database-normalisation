# Database-Normalisation

## Introduction
**What is Normalization?**
Normalization is the process of organizing the data in the database. Normalization divides the larger table into smaller and links them using relationships.

A large database defined as a single relation may result in data duplication. This repetition of data may result in:
- Wastage and poor utilization of disk space and resources.
- It makes it difficult to maintain and update data as it would involve searching many records in relation.
- The likelihood of errors and inconsistencies increases.
 
**Why do we need Normalization?** 
- Normalization is used to minimize the redundancy from a relation or set of relations.
- Normalization is used to eliminate undesirable characteristics like Insertion, Update, and Deletion Anomalies.

 **What is Insertion, Update, and Deletion Anomalies**
 - **Insertion Anomaly** refers to when one cannot insert a new tuple into a relationship due to lack of data.
 - **Deletion Anomaly** The delete anomaly refers to the situation where the deletion of data results in the unintended loss of some other important data.
 - **Updatation Anomaly** The update anomaly is when an update of a single data value requires multiple rows of data to be updated.

  ## Types of Normal Forms:

  ### First normal Form
  A relation is in first normal form if every attribute in that relation is single-valued attribute. If a relation contains a composite or multi-valued attribute, it violates the first normal form.
   The table below is not in first normal form since courses column is a multivalued attribute
   
![q](https://github.com/allan-pg/database-normalisation/assets/62595869/67d6343b-5dc3-4db5-acc1-e8b3fcb7642d)

for it to be in first normal form there is no multi-valued attribute:

![q](https://github.com/allan-pg/database-normalisation/assets/62595869/35078de7-6696-4a18-a1b3-937727a5e3cd)

For a table to be in first normal form:
- makes sure that there are no recurring groups inside rows.
- Ensure all of a table’s columns contain atomic values, or indivisible values that is, each column can have only one value for each row in the table.
- there must be a primary key for identification.
- Field names soud be distinct.

### Second normal form
The second step is to eliminate redundant data and get into second normal form. If attributes are not dependent on the primary key, place them into a separate entity. 

For a table to be in normal form
- The table satisfies 1NF (first normal form).
- Non-primary key attributes depend on all attributes of a composite key.

### Tird Normal Form
The third normal form applies to a table if
- The table meets the criteria for 2NF.
- Each nonprimary key attribute in a row does not depend on the entry in another key column.

  ## Advantages of Normalization
  - Normalization helps to minimize data redundancy
  - Data consistency within the database.
  - Enforces the concept of relational integrity.
  - Greater overall database organization.

   ## Disadvantages of Normalization
   - It is very time-consuming and difficult to normalize relations of a higher degree.
   - The performance degrades when normalizing the relations to higher normal forms, i.e., 4NF, 5NF.


 ## conclusion
 Failure to eliminate anomalies leads to data redundancy and can cause data integrity and other problems as the database grows.
