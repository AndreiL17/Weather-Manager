## Technologies Used
 ### The backend uses  Java 17. The libraries used are:

- Spring Boot
- Lombok: For generating getters, setters, constructors at compile time
- MariaDB: Since it uses SQL for defining, querying, and managing data
- Flyway: Helps with database configuration through things like version control, consistency across environments
- OpenCSV: Library used to write CSV files
- JavaTuples: Provides tuple classes for convenience
- Maven Plugin: 
    * maven-compiler-plugin: Configured to use lombok annotation processor and compile the code to Java
    * spring-boot-maven-plugin: packages the application as a JAR


### The frontend employs Typescript with React. The library used are:
 
- React and React Router: form the core of our UI and client-side routing
- Vite: Build tool and development server
- ESLint: for code quality and consistency in style
- Typescript definitions: type support for the React libraries

This configuration includes multiple benefits such as: fast build times, robust UI features, code quality checks.

## Maturity of the Api

Our API easily clears Level 0 Maturity, as it clearly makes use of HTTP methods as a way of completing transactions between
user and server. At this level, data can be represented in any way, but there is the option between CSV and JSON.

Level 1 enforces that resources have to be identified by URIs, which is present. Now, interactions target specific resources, such as through our filtering methods using GET, but also the way that our pages are layed out, each being accessible through URLs from the home page.

Level 2 is also respected in our application, requiring the use of HTTP verbs, as well as the generation of status codes. These are not only done 
through our endpoints, retrieving data, posting, editing, and manipulating it for the clarity of the user, but also employ complete and clear
status codes, making use of the concept of self-describing messages.

However, the last level would require the application to provide more links and hypermedia controls, which is not something that is currently implemented.
This last level is a big step which includes. There are some links binding resources between them, but a full Level 3 API would need every resource
to be accessible from any point, and do it in a simple manner, as users should be able to navigate the application through hypermedia links without
having to know its structure beforehand.


