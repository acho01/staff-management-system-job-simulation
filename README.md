# Staff Management System API (Job Simulation)

The project is divided into 3 different parts:
- Easy( Fixing project setup issues, adding dependencies, fixing already existing bugs in the controller )
- Medium( Implement basic functionality of the system: Design API, design Database structure, design a usecase architecture of components,
Test it ).
- Hard( Implement more complex features, deploy to cloud )

# General project info

In the scope of this project you will be building a simple version of staff management system. In general staff management system is a platform that contains information about all employees in the company along side with projects that they are assigned to. Availability, personal information, holiday management etc. The interesting part of the project is user - user role/group relation. For instance users in ADMIN user group will only have the permission to add, delete and update data. You can also have a SIMPLE(you can name it differently) user which will only be able to read some data from the platform.
You will start from the basics and step-by-step get to the real production grade solution. If you work hard and keep consistent the project will give you real working experience which is very hard to gain even at some production projects. So without farther ado let's start and get your hand dirty with coding some real system.

# Overview of Features/requirements to complete/implement from scratch 
### You can call it the first part of your job simulation, or as they call in Agile development your first Sprint that will contain a mini version of the system.

- Fix, implement and test User CRUD API (At this stage you will not be using real database as storage. In-memory storage will be used)
  - POST method for creating new user
  - GET method for getting user by id
  - DELETE method for deleting user with specified id
  - UPDATE method for updating different fields of the user
- Introduce a user role/group notion in the platform. Create CRUD api for user role/group. Implementation should mimic the in-memory
storage structure just like the users.
- Refactor User API and tests to work with User Role/Group concept. User's that have no permission to update data should not be able to do that.

### The second part of the platform will consist of creating the core functionality and adding some new interesing features from scratch. Congratualtions, this is your second Sprint, keep working!!!

- Refactor code to the layered architecture
- Setup ORM and database connection
- Refactor your code to use database with ORM instead of in-memory storage (At this point if architecture is imlemented smoothly you will notice how easily this process will be done)
- Create detailed database table structure, including already existing entities as well as every other entity that will be added for new features.
- Introduce project notion, and try to build logic around assigning users to the projects, the time ranges, full-time or part-time availability etc
- Create a user hierarchy system, every user, besides root user, should have a "manager" to whom he will be reporting. The use case of this feature can be vacation requests.
- Based on previous idea, you will be asked to implement holiday/vacation management syb-system. If a user wants to take a 1 day vacation(day-off) or a multiple day vacation, he/she should create a request to his "manager" and wait for the approval from him/her.

### On the final stage, you will spend least time coding and more thinking about infrastructure and deployment

- As you are going to deploy the API on cloud, you will not want to let everyone use it. You will add/implement a functionality that will give access to specific clients to use your API
- Dockerize your application, setup instance on cloud and deploy your project
- Setup CI/CD to automatically update and deliver changes to the cloud

# Interesting optional extensions 

- Introduce Company notion in the system. In this feature you will have to slightly refactor the architecture and maybe add some additional features that can be attractive for the company. Basic idea is to enable creating different platforms for multiple companies, rather than sticking with a single company solution.

# Technologies used
- [Java](https://docs.oracle.com/en/java/javase/11/docs/api/): Java programming language
- [Spring Boot](https://spring.io/projects/spring-boot): Most famous framework for building server applications on java
- [PostgresSQL](https://www.postgresql.org/docs/current/index.html): Very popular and battle tested Relational type of database
- [Hibernate](https://hibernate.org/): Most popular JPA implementation. Battle tested framework to work with databases from java.
- [Docker](https://docs.docker.com/get-started/): Containerization mechanism to easily test, deploy and orchestrate application units.
- [DigitalOcean](https://www.digitalocean.com/): Vey popular cloud service provider, easy to use. Great for this kind of educational projects.

#

This is the basic overview of the project. For sure you are free to add different functionality, but it's better to think of it after delivering the working solution. The consistent following of the plan is also a great skill to take from here. 
Testing and documenting part of the project is not mentioned above, because it's just as natural as coding. All the details and resources will be shared with you in the issues section above. What's great about this project is that you will be treated as a real employee, creating Pull-Requests and receiving code reviews from our team. Consistency is the key to get maximum from this opportunity. 
Good Luck !!!
