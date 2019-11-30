# Normalization vs Denormalization

**Normalization** is about trying to increase data integrity by reducing the number of copies of the data. Data that needs to be added or updated will be done in as few places as possible.

**Denormalization** is trying to increase performance by reducing the number of joins between tables \(as joins can be slow\). Data integrity will take a bit of a potential hit, as there will be more copies of the data \(to reduce JOINS\).

> ⚠A transitive dependency in a database is an indirect relationship between values in the same table that causes a [functional dependency](https://www.lifewire.com/functional-dependency-definition-1019257). To achieve the normalization standard of [Third Normal Form](https://www.lifewire.com/normalizing-your-database-third-1019726) \(3NF\), you must eliminate any transitive dependency.

This blog explains what is transitive dependency. Click [Here](https://www.lifewire.com/transitive-dependency-1019760#:~:targetText=A%20transitive%20dependency%20in%20a,must%20eliminate%20any%20transitive%20dependency)



