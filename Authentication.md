# Class 06

**Authentication** is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know

**Session Management** is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict. 

**User IDs**
Make sure your usernames/user IDs are case-insensitive. User 'smith' and user 'Smith' should be the same user. Usernames should also be unique. For high-security applications, usernames could be assigned and secret instead of user-defined public data.

**Authentication Solution and Sensitive Accounts**
- Do NOT allow login with sensitive accounts (i.e. accounts that can be used internally within the solution such as to a back-end / middle-ware / DB) to any front-end user-interface
- Do NOT use the same authentication solution (e.g. IDP / AD) used internally for unsecured access (e.g. public access / DMZ)

## Research

**Explain what a “Singleton” is (in Computer Science terms)?**

A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.

**Explain how the Singleton pattern can be used with Node modules, specifically with classes?**

We need singleton when we want to make sure there is only one object instantiated. Therefore, instead of creating a new object we need to ensure the constructor was called only once and then we reuse the instance.
We can achieve this by refactoring our class to have:
- hidden (private)constructor
- public getInstance method that returns instance of the class

## Term

**router middleware:** is bound to an instance of a router or Express.router(). This means the middleware will be applied to only the API endpoints defined in a specific instance of Express.router(). That being said, a router-middleware would execute additional logic in a file like teams.routes.ts, which contains only /api/teams related API endpoints.

**Dynamic Module Loading:**is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory. It is one of the 3 mechanisms by which a computer program can use some other software; the other two are static linking and dynamic linking. Unlike static linking and dynamic linking, dynamic loading allows a computer program to start up in the absence of these libraries, to discover available libraries, and to potentially gain additional functionality.

**Singleton Pattern:**s a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.

**CRUD -> REST Method Matches:**is request methods to indicate the desired action to be performed for a given resource. Although they can also be nouns, these request methods are sometimes referred to as HTTP verbs. Each of them implements a different semantic, but some common features are shared by a group of them: e.g. a request method can be safe, idempotent, or cacheable.

**Mock Testing:**is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. The purpose of mocking is to isolate and focus on the code being tested and not on the behaviour or state of external dependencies.



## Securing Passwords

Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords.

### weaknesses of cryptographic hash algorithm that allows an attacker to calculate the original value of a hashed password :
- **Brute Force attack** : Hashes can't be reversed, so instead of reversing the hash of the password, an attacker can simply keep trying different inputs until he  find  the same hash value, called brute force attack.
- **Hash Collision attack** : Hash functions have infinite input length and a predefined output length, so there is inevitably going to be the possibility of two different inputs that produce the same output hash. MD5, SHA1, SHA2 are vulnerable to Hash Collision Attack i.e. two input strings of a hash function that produce the same hash result.

**BCrypt, IT's SLOW AND STRONG AS HELL**

To overcome such issues, we need algorithms which can make the brute force attacks slower and minimize the impact. Such algorithms are PBKDF2 and BCrypt, both of these algorithms use a technique called Key Stretching.

### Basic Auth

In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon : .
