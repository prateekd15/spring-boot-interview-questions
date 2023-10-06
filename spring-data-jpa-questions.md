# Spring Data JPA Interview Questions

## Table of Contents
| Questions                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [What is Spring Data JPA, and how does it differ from traditional JPA?](what-is-spring-data-jpa-and-how-does-it-differ-from-traditional-jpa)|
| [Spring Data JPA Interview Questions](spring-data-jpa-questions.md)|


## What is Spring Data JPA, and how does it differ from traditional JPA?

Spring Data JPA builds on top of the Java Persistence API (JPA) and adds a layer of abstraction and convenience for working with databases. It simplifies the data access code in your Spring applications, reduces boilerplate code, and promotes best practices. However, it's important to note that Spring Data JPA does not replace JPA but rather enhances and streamlines its usage within Spring-based applications.

Here are the key aspects of Spring Data JPA and how it differs from traditional JPA:

1. **Simplified Data Access**: Spring Data JPA simplifies the data access layer by reducing the amount of boilerplate code you need to write. It provides repositories and query methods that allow you to perform common database operations (like CRUD operations) without writing explicit SQL or JPQL queries.

2. **Repository Interface**: In Spring Data JPA, you define data repositories using interfaces that extend the `JpaRepository` interface or its subinterfaces. These interfaces automatically provide basic database operations such as save, delete, and find, based on the entity type and method naming conventions.

3. **Custom Query Methods**: Spring Data JPA allows you to define custom query methods in your repository interfaces by following a naming convention. You can name your methods in a specific way, and Spring Data JPA will automatically generate the corresponding SQL or JPQL queries at runtime.

4. **Pagination and Sorting**: Spring Data JPA provides built-in support for pagination and sorting of query results, making it easy to implement paginated data views.

5. **Native Queries and JPQL Support**: While Spring Data JPA encourages the use of query methods with naming conventions, it also allows you to write native SQL queries or JPQL queries when you need more complex or custom queries.

6. **Automatic Query Execution**: Spring Data JPA automatically translates repository method calls into corresponding SQL or JPQL queries and executes them. This automation reduces the need for writing explicit query code.

7. **Integration with Spring Framework**: Spring Data JPA seamlessly integrates with the Spring Framework, providing additional benefits like transaction management, dependency injection, and more.

8. **Support for Different Data Sources**: Spring Data JPA can work with various data sources, not just relational databases. It supports MongoDB, Cassandra, Neo4j, and other data stores through separate Spring Data modules.

9. **Custom Repository Implementations**: If needed, you can provide custom implementations for your repository interfaces to handle more complex data access logic.