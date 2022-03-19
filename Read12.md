# Spring RESTful Routing & Static Files

## What is JPA
#### JPA (Java Persistence API): JPA is a specification. It is a collection of classes and methods to persistently store the vast amounts of data into a database. It provides common prototype and functionality to ORM tools. By implementing the same specifiation, all ORM tools (like Hibernate, TopLink..) follows the common standarts.

[Here is most full Practice to Learn how to Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)





## REPOSITORY
#### Now it is time to create a Person Repository. This repository holds each person to be added to the system. We will create a PersonRepository interface and it will extend JPA Repository class. JPA repository has many functions that we can use for database operations.
#### JpaRepository is a JPA (Java Persistence API) specific extension of Repository. It contains the full API of CrudRepository and PagingAndSortingRepository. So it contains API for basic CRUD operations and also API for pagination and sorting.
[Example](https://www.baeldung.com/spring-data-repositories)
