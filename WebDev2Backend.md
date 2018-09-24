## Web Dev 2: Backend
### Presenter: Michal Jez

**Target Audience:** 
- People with basic programming and web experience

**Suggested Prerequisites:** 
- Knowledge of JavaScript
- MySQL, Node & Postman installed

**Workshop Goals:**

- To build a simple To-Do list API

**Description:**

This workshop aims to teach the basic concepts behind a simple REST API such as wiring up endpoints with Express.js, persisting data in a database with MySQL and interfacing with that data through Sequelize.js. It will also cover authentication through JWTs and other topics such as CORS. The end result will be a fully functional To-Do list api implementing all of the above.

**Content Breakdown:**

- Intro
    - Learning goals
    - Outline
    - Technologies used
- REST
    - What is REST (2)
    - GET/PUT/POST/DELETE (3)
    - Create endpoints with express (10)
- Data storage
    - DBs/file system/in memory storage
    - Types of DBs (5)
    - Wiring up MySQL with sequelize (10)
- Application design
    - Authentication (10)
    - CORS (5)

**[Slides](https://docs.google.com/presentation/d/1oZ3Bo68pcz8M7gjnVHfCEn5CRYhxyAtFYzg3hAbD1y4/edit?usp=sharing)**

---

**Key Notes:**
* What is an API
    * REST: REpresentational State Transfer
    * 4 common requests
        * GET: Fetches a resource from the server
        * POST: Creates a resource on the server
        * PUT: Updates a resource on the server
        * DELETE: Deletes a resource from the server
    * Parts of a url
        * Protocol
        * Host
        * Path
        * Query params
        * Headers
        * Cookies
        * Body
    * Common endpoint layout
    * Todo list endpoint layout
    * Walk through barebones express app

* Data storage
    * In memory
        * Pros
            * Fast access
            * Simple to wire up
        * Cons
            * Limited memory
            * Storage doesn’t persist if server crashes
    * File system
        * Pros
            * HDDs and SSDs are cheaper than RAM
            * Easy way to store files
        * Cons
            * Not easy to query
            * Horizontal scalability issues
    * Database
        * Pros
            * Data persists
            * Built to be fast
        * Types
            * Relational (SQL)
                * Comprised of tables which you can join using foreign keys
                * Queryable using the Standard Query Language
                * MySQL, Postgres
            * Non-relational
                * MongoDB
    * ORM
        * Object-relational mapping
        * An interface between tables in a database and objects in your programming language
        * Helps with building queries
            * Can prevent SQL injection attacks

* Application Design
    * CORS
        * Cross-origin resource sharing
        * Used when a page on domain-a.com makes a request to a server on domain-b.com
        * CORS works by adding additional headers to an OPTIONS request sent by your browser such as setting which origins requests can come from and which request methods are valid
    * Authentication
        * Authentication is usually performed by sending an authentication token with a request
        * JWT: JSON Web Token
            * Stateless
            * Contains 3 sections [header].[payload].[hash]
            * Doesn’t need to be stored on the server
