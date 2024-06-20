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
