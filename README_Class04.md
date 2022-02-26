## Question

**Name 3 advantages to Test Driven Development?**

1- THE SOFTWARE DESIGN BECOMES MODULAR

2-  THE CODE IS EASIER TO MAINTAIN

3-  CODE REFACTORING GOES MORE SMOOTHLY

**In what case would you need to use beforeEach() or afterEach() in a test suite?**

The before and after will run before and after the execution of the test suite respectively (in our case, the test-file), while beforeEach and afterEach are ran before and after each test case (test step).

**What is one downside of Test Driven Development?**
- No silver bullet
- slow process
- all the members of a team got to do it 

**What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

JavaScript classes, introduced in ECMAScript 2015, are primarily syntactical sugar over JavaScript's existing prototype-based inheritance. The class syntax does not introduce a new object-oriented inheritance model to JavaScript.

**Why REST?**


1- REST is Easy to Understand and Implement

2- REST Makes your Application More Scalable

3- Caching is Easier with REST

4- REST is Flexibile


## Term

**functional programming:**
is a programming paradigm designed to handle pure mathematical functions. This paradigm is totally focused on writing more compounded and pure functions.

**Object-oriented programming (OOP):**
 is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.

 **Class:**
 an abstract blueprint used to create more specific, concrete objects. Classes often represent broad categories, like Car or Dog that share attributes

 **Super:** keyword is used to access and call functions on an object's parent.

 **this:** the this keyword usually reffers to the object that called the function, but in es5, the bind method was introduced to set the value of the function's this regardless of how it is called.

 **Test Driven Development (TDD):**
a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

 **Jest:**
 JavaScript testing framework with a focus on simplicity and support for large web applications. It works with projects using Babel, TypeScript, Node.js, React, Angular, Vue.js and Svelte.

 **Continuous Integration (CI):**
the practice of automating the integration of code changes from multiple contributors into a single software project.

 **REST:**
REpresentational State Transfer, is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other. REST-compliant systems, often called RESTful systems, are characterized by how they are stateless and separate the concerns of client and server.

 **Data Model:**
an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities.

## Preview

**Which 3 things had you heard about previously and now have better clarity on?** 

NO, it is a new information for me.
**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

I hope to know more about the middleware 
**What are you most excited about trying to implement or see how it works?**

 Middleware

 ## SQL vs NoSQL

 **SQL** is the programming language used to interface with relational databases. (Relational databases model data as records in rows and tables with logical links between them).

 **NoSQL** is a class of DBMs that are non-relational and generally do not use SQL.

**SQL vs NoSQL:**

- SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.
- SQL databases are table based databases whereas NoSQL databases are document based.
- SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
- SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable.
- SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents.
- SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb.
- For complex queries: SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries.

**SQL modeling techniques**
the SQL modeling depends on what is the relation between tables one to one relation. one to many relation. many to one relation. many to many relation.

for this modeling the method is normalizaion for the database.

**Sequalize**

Sequelize is a promise-based Node.js ORM tool for Postgres, MySQL, MariaDB, SQLite, Microsoft SQL Server, Amazon Redshift and Snowflake’s Data Cloud. It features solid transaction support, relations, eager and lazy loading, read replication and more.
