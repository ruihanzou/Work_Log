---
description: Introduce the concepts of Normalization and Denormalization
---

# Normalization vs Denormalization

1. **How to reach First Normal Form \(1NF\):** 
   * Atomic values: each cell contains unique and single values 
   * Be able to add data without altering tables 
   * Separate different relations into different tables 
   * Keep relationships between tables together with foreign keys
2. **Second Normal Form \(2NF\):** 
   * Have reached 1NF
   * All columns in the table must rely on the Primary Key
3. **Third Normal Form \(3NF\):**  


   * Must be in 2nd Normal Form
   * No transitive dependencies
   * Remember, transitive dependencies you are trying to maintain is that to get from A-&gt; C, you want to avoid going through B.

   **When to use 3NF:**

   * When you want to update data, we want to be able to do in just 1 place. We want to avoid updating the table in the Customers Detail table \(in the example in the lecture slide\).

**Normalization** is about trying to increase data integrity by reducing the number of copies of the data. Data that needs to be added or updated will be done in as few places as possible.

**Denormalization** is trying to increase performance by reducing the number of joins between tables \(as joins can be slow\). Data integrity will take a bit of a potential hit, as there will be more copies of the data \(to reduce JOINS\).

> ⚠A transitive dependency in a database is an indirect relationship between values in the same table that causes a [functional dependency](https://www.lifewire.com/functional-dependency-definition-1019257). To achieve the normalization standard of [Third Normal Form](https://www.lifewire.com/normalizing-your-database-third-1019726) \(3NF\), you must eliminate any transitive dependency.

This blog explains what is transitive dependency. Click [Here](https://www.lifewire.com/transitive-dependency-1019760#:~:targetText=A%20transitive%20dependency%20in%20a,must%20eliminate%20any%20transitive%20dependency)



