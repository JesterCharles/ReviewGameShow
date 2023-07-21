# Spring Boot Competency

<details>
<summary> Spring Core Framework</summary>

### 100: Spring Framework:

**Definition:** Spring Framework is an open-source, lightweight, and comprehensive application framework for Java. It provides a robust platform for building enterprise-level applications by offering features such as dependency injection, aspect-oriented programming, data access, transaction management, and more.

**Importance:** Spring Framework simplifies Java development by promoting modular, reusable, and testable code. It encourages best practices like loose coupling and separation of concerns, leading to more maintainable and scalable applications.

**Use cases:** Spring Framework is used for developing a wide range of applications, from small web applications to large enterprise-level systems. It is commonly used in web development, RESTful services, batch processing, and integration with various technologies and frameworks.

### 200: Dependency Injection:

**Definition:** Dependency Injection (DI) is a design pattern and core concept in the Spring Framework. It is the process of providing the dependent objects (dependencies) of a class externally, instead of letting the class create them itself. This allows for loose coupling between classes and improves code flexibility.

**Importance:** Dependency Injection promotes the principle of Inversion of Control (IoC) and enhances the maintainability and testability of applications. It reduces the complexity of managing object dependencies and makes code more modular and flexible.

**Use cases:** Dependency Injection is used throughout the Spring Framework for managing and configuring dependencies between Spring beans. It allows developers to easily switch implementations, inject mock objects for testing, and manage complex object graphs in large applications.

### 300: Inversion of Control:

**Definition:** Inversion of Control (IoC) is a design principle in software development where the control over the flow of a program is shifted from the program itself to an external container or framework. In the context of Spring, IoC means that the Spring container manages the instantiation, configuration, and lifecycle of objects.

**Importance:** IoC enables loose coupling and facilitates the integration of different components within an application. It promotes modular design, easier testing, and flexibility in changing implementations without modifying the application code.

**Use cases:** IoC is a foundational concept in the Spring Framework, where it manages the creation and assembly of objects (beans) and handles their lifecycle. It is used throughout the framework, allowing developers to focus on business logic rather than managing object creation and wiring.

### 400: ApplicationContext:

**Definition:** ApplicationContext is a core interface in the Spring Framework that represents the Spring IoC container. It is responsible for managing the configuration of Spring beans and providing access to them during the application's runtime.

**Importance:** ApplicationContext is a key component of Spring as it handles object instantiation, dependency injection, and provides a wide range of services like event propagation, internationalization, and resource management.

**Use cases:** The ApplicationContext is used throughout Spring applications to retrieve beans, manage their lifecycle, and access various Spring services. It is typically created and managed by the Spring container to handle the application's bean management.

### 500: Components of Spring Framework:

**Definition:** The Spring Framework is composed of several key components, including Core Container, Data Access/Integration, Web, AOP (Aspect-Oriented Programming), and Test. Each component provides specific functionalities that cater to different aspects of Java application development.

**Importance:** The various components of Spring work together to create a comprehensive and modular framework that covers a wide range of application development needs. Developers can choose and integrate the required components as per the application's requirements.

**Use cases:** The Core Container provides the foundational features like DI and IoC, the Data Access/Integration component facilitates database access and integration, the Web component handles web-related functionalities, AOP manages cross-cutting concerns, and the Test component assists in unit testing and integration testing. Developers can utilize these components to build various types of applications, including web applications, enterprise systems, and RESTful services.
</details>

<details>
<summary>Beans</summary>

### 100: Bean in Spring:

**Definition:** In Spring, a bean is an object that is managed by the Spring IoC container. It is created, configured, and assembled by the container based on the information provided in the Spring configuration files or annotations.

**Importance:** Beans are the building blocks of Spring applications. They represent various components, services, and objects that form the core functionality of the application. The Spring container manages the lifecycle and dependencies of beans, promoting loose coupling and modular design.

**Use cases:** Beans are used to represent various components in a Spring application, such as controllers, services, data access objects, and more. They can be configured with different scopes, dependencies, and properties to cater to different application requirements.

### 200: Scopes of a Bean:

**Definition:** The scope of a bean in Spring defines the lifecycle and visibility of the bean instance within the container. Spring provides different bean scopes, each serving specific purposes.

**Importance:** Scopes determine how long a bean instance lives and how it is shared among different components. Understanding and configuring the appropriate scope is essential for managing resource usage and maintaining the correct state of beans.

**Use cases:** Different scopes are used for different scenarios. For example, singleton scope is used when you want a single shared instance across the entire application, prototype scope is used when you need a new instance each time the bean is requested, and other scopes like request, session, and custom scopes are used in web applications for managing bean instances within the scope of HTTP requests or sessions.

### 300: Injecting Beans:

**Definition:** Injecting beans in Spring refers to the process of providing dependencies to a bean by the Spring IoC container automatically. This is achieved through dependency injection, where the container wires the required dependencies into the bean.

**Importance:** Dependency injection is a fundamental concept in Spring, promoting loose coupling and reducing the need for direct object creation and management. It simplifies object composition and makes it easier to switch implementations and perform unit testing.

**Use cases:** Injecting beans is used whenever a bean requires other beans or objects to perform its functionality. It is common in scenarios where you want to compose complex objects from smaller components or when collaborating with other services.

### 400: Bean Lifecycle:

**Definition:** The bean lifecycle in Spring represents the different stages a bean goes through from its creation to its destruction. It includes various lifecycle callbacks, such as initialization and destruction, where custom logic can be executed.

**Importance:** Understanding the bean lifecycle is crucial for managing resources and performing actions during specific phases of a bean's existence. It allows developers to control the initialization and cleanup processes of beans effectively.

**Use cases:** Bean lifecycle callbacks are used to perform tasks like initializing database connections, closing resources, and setting up configurations during bean creation or cleanup. They are often used in conjunction with Spring's InitializingBean and DisposableBean interfaces or through custom annotations.

### 500: Bean Wiring:

**Definition:** Bean wiring in Spring refers to the process of connecting different beans and managing their dependencies within the Spring IoC container. This is achieved through configuration files, annotations, or Java-based configuration.

**Importance:** Bean wiring is a fundamental aspect of Spring that facilitates loose coupling and modularity. It allows developers to define how different beans interact and collaborate without the need for manual instantiation or object management.

**Use cases:** Bean wiring is used to establish relationships between beans, such as injecting dependencies, setting up cross-cutting concerns using AOP, and configuring beans to be aware of each other within the application context. It is a critical aspect of building complex applications with Spring's powerful component management capabilities.
</details>

<details>
<summary> Spring Boot</summary>

### 100: Spring Initializr:

**Definition:** Spring Initializr is a web-based tool provided by the Spring team to generate a basic Spring Boot project structure with specific dependencies. It allows developers to quickly bootstrap Spring projects by selecting dependencies, project settings, and packaging options.

**Importance:** Spring Initializr simplifies the process of starting a new Spring Boot project. It ensures that the necessary dependencies and configurations are correctly set up, enabling developers to focus on building the application's business logic.

**Use cases:** Spring Initializr is used when starting a new Spring Boot project. Developers can use it to select specific dependencies based on the project's requirements and generate a project structure that follows best practices and Spring Boot conventions.

### 200: application.properties or .yml:

**Definition:** `application.properties` and `application.yml` are configuration files in Spring Boot. They allow developers to specify various configuration properties for the application, such as database settings, logging levels, and external service configurations.

**Importance:** These configuration files provide flexibility in customizing the application's behavior without modifying the source code. They make it easier to configure different environments (e.g., development, testing, production) without rebuilding the application.

**Use cases:** `application.properties` or `application.yml` are used to set up various properties required for the application. They are used to configure data source connections, logging levels, profiles, and other application-specific settings.

### 300: Embedded server in Spring Boot:

**Definition:** Spring Boot offers an embedded server by default, allowing developers to run web applications without requiring a separate web server (e.g., Tomcat or Jetty). The embedded server is included in the application's jar file or war file.

**Importance:** The embedded server simplifies deployment and distribution of Spring Boot applications. It reduces the complexity of managing an external web server and makes it easier to package the application as a standalone executable.

**Use cases:** The embedded server is used whenever a Spring Boot application needs to be deployed as a self-contained executable. It is commonly used in web applications, RESTful APIs, and microservices.

### 400: @SpringBootApplication:

**Definition:** @SpringBootApplication is a meta-annotation in Spring Boot that combines several annotations, including @Configuration, @EnableAutoConfiguration, and @ComponentScan. It is typically used at the main class to bootstrap a Spring Boot application.

**Importance:** @SpringBootApplication reduces boilerplate code by combining multiple annotations into one. It enables auto-configuration and component scanning, making it easier to set up and configure a Spring Boot application.

**Use cases:** @SpringBootApplication is used at the main class of a Spring Boot application. It is essential for bootstrapping the application and enabling automatic configuration and component scanning.

### 500: Spring Core vs. Spring Boot:

**Definition:** Spring Core is the foundational module of the Spring Framework, providing features like dependency injection, aspect-oriented programming, and more. Spring Boot, on the other hand, is a separate project that builds on top of Spring Core and aims to simplify the configuration and setup of Spring applications.

**Importance:** Spring Core provides the fundamental features for building enterprise-level applications with dependency injection and aspect-oriented programming. Spring Boot streamlines the development process by providing auto-configuration and sensible defaults, reducing boilerplate code and allowing developers to focus on business logic.

**Use cases:** Spring Core is used to build Spring applications with fine-grained control over configurations and component management. Spring Boot is used when rapid development and easy setup of Spring applications are desired, especially for building microservices and web applications.
</details>

<details>
<summary> Spring Additional</summary>

### 100: Spring DevTools:

**Definition:** Spring DevTools is a module in the Spring Framework that provides a set of development-time features aimed at improving the developer's productivity. It includes functionalities like automatic application restart, remote debugging support, and enhanced developer tools.

**Importance:** Spring DevTools is essential for rapid development and debugging in a Spring-based application. It reduces development time by automatically reloading the application when changes are made, making the development process more efficient.

**Use cases:** Spring DevTools are used during development to streamline the application development process. It is particularly useful when you want to see immediate changes without the need to redeploy the entire application manually.

### 200: Spring Environment:

**Definition:** The Spring Environment is an abstraction that represents the environment in which a Spring application is running. It provides access to configuration properties, profiles, and other system-specific information.

**Importance:** The Spring Environment allows developers to configure and customize their applications based on the specific runtime environment. It helps in creating flexible and configurable applications that can adapt to different deployment scenarios.

**Use cases:** The Spring Environment is used to retrieve configuration properties, manage profiles, and access system environment variables. It is commonly used when you want to configure different behavior based on the deployment environment, such as development, testing, or production.

### 300: Spring Actuator:

**Definition:** Spring Actuator is a module in the Spring Framework that provides production-ready features to monitor and manage applications. It exposes various endpoints and metrics to monitor the health, performance, and state of a Spring application.

**Importance:** Spring Actuator is crucial for monitoring and managing the health and performance of a Spring application in production environments. It provides insights into application internals and helps diagnose and troubleshoot issues effectively.

**Use cases:** Spring Actuator is used in production environments to gain insights into the application's health, check system information, and monitor various metrics like CPU usage, memory consumption, and request statistics. It is beneficial for DevOps teams and system administrators to monitor and manage deployed applications.

### 400: Stereotype Annotations:

**Definition:** Stereotype annotations in Spring are a set of specialized annotations used to indicate the roles or behavior of certain classes within a Spring application. They include annotations like @Component, @Service, @Controller, and @Repository.

**Importance:** Stereotype annotations help in organizing and configuring Spring beans in a more structured manner. They allow the Spring container to automatically detect and register beans based on their roles or behaviors, reducing the need for explicit configuration.

**Use cases:** Stereotype annotations are used to identify and categorize beans based on their responsibilities. For example, @Service is used for service layer components, @Controller for web controllers, and @Repository for data access objects. Using these annotations, you can easily organize and configure beans in Spring applications.

### 500: Risks involved with Spring Actuator:

**Definition:** While Spring Actuator is a powerful tool for monitoring and managing Spring applications, there are certain risks associated with its use. Exposing sensitive endpoints or information through Actuator could potentially lead to security vulnerabilities.

**Importance:** It is crucial to carefully configure Spring Actuator and limit access to sensitive endpoints to prevent unauthorized access or information leakage. Misconfigured Actuator endpoints could expose sensitive system information or allow attackers to perform harmful actions on the application.

**Use cases:** The risks associated with Spring Actuator are relevant when deploying Spring applications in production environments. It is essential to properly configure Actuator endpoints, restrict access to authorized users, and ensure that sensitive information is not exposed to the public. Regular security audits and monitoring of Actuator endpoints are recommended to mitigate potential risks.
</details>

<details>
<summary>Spring Web MVC</summary>

### 100: @RestController:

**Definition:** @RestController is a specialized annotation in Spring that combines @Controller and @ResponseBody annotations. It is used to define a controller class that handles incoming HTTP requests and returns the response directly in the desired format (typically JSON or XML) without the need for a view resolver.

**Importance:** @RestController simplifies the development of RESTful web services by eliminating the need for additional annotations to indicate the response format. It is widely used for building RESTful APIs that return data in JSON or XML format.

**Use cases:** @RestController is used in Spring applications to define controller classes that handle RESTful API requests. It is commonly used in web applications, microservices, and other scenarios where you want to build APIs for client-server communication.

### 200: Spring MVC:

**Definition:** Spring MVC (Model-View-Controller) is a web framework within the Spring Framework that provides an architectural pattern for building web applications. It separates the application into three components: Model (data), View (user interface), and Controller (request handling logic).

**Importance:** Spring MVC simplifies web application development by providing a structured and modular approach. It promotes separation of concerns, making code more maintainable and testable. It also supports various view technologies and integration with other Spring features.

**Use cases:** Spring MVC is used for building web applications that follow the Model-View-Controller pattern. It is widely used in web development, providing a robust framework for handling HTTP requests, managing session and application data, and rendering dynamic content.

### 300: @RequestParams:

**Definition:** @RequestParams is a Spring annotation used to extract request parameters from the URL or query parameters. It binds the values of request parameters to the method parameters in a controller's request-handling method.

**Importance:** @RequestParams simplifies the process of extracting data from the request URL and automatically converting them to the appropriate Java data types. It is useful for processing form submissions and handling request data.

**Use cases:** @RequestParams is used in Spring MVC controllers to extract and process request parameters. It is commonly used in scenarios where you need to pass data to the server through the URL or query parameters, such as search queries or form submissions.

### 400: ResponseEntity:

**Definition:** ResponseEntity is a generic class in Spring used to represent an HTTP response. It allows you to customize the response status, headers, and body of the HTTP response returned by a controller method.

**Importance:** ResponseEntity provides fine-grained control over the HTTP response, making it useful when you need to handle specific HTTP status codes, set custom headers, or return different response bodies based on business logic.

**Use cases:** ResponseEntity is used in Spring MVC controllers when you want to create custom HTTP responses with specific status codes, headers, and response bodies. It is often used in RESTful APIs to return data along with appropriate HTTP status codes and headers.

### 500: DispatcherServlet:

**Definition:** DispatcherServlet is the front controller in Spring MVC applications. It receives incoming HTTP requests and delegates them to the appropriate handler methods (controllers) based on the request mapping and configuration.

**Importance:** DispatcherServlet plays a crucial role in the Spring MVC architecture. It centralizes the request handling and helps in managing the flow of incoming requests through the application, making it easier to handle different types of requests and perform necessary pre- and post-processing.

**Use cases:** DispatcherServlet is used in Spring MVC applications to handle incoming HTTP requests and route them to the appropriate controllers. It is a fundamental component of Spring MVC that enables the separation of concerns and the efficient handling of web requests.
</details>

<details>
<summary> Spring Data JPA</summary>

### 100: JPA Repository:

**Definition:** JPA Repository is a feature provided by Spring Data JPA that provides a higher-level abstraction for interacting with a relational database. It is an interface that extends the JpaRepository interface and inherits various CRUD (Create, Read, Update, Delete) methods for database operations.

**Importance:** JPA Repository simplifies database access by eliminating the need for writing custom SQL queries or DAO classes. It provides a consistent and easy-to-use API for performing common database operations.

**Use cases:** JPA Repository is used when you want to interact with a relational database in a Spring application. It is commonly used for handling CRUD operations and custom queries in Spring Data JPA.

### 200: JPA:

**Definition:** JPA (Java Persistence API) is a specification that defines a standard way to manage relational data in Java applications. It provides an object-relational mapping (ORM) mechanism, allowing developers to map Java objects to database tables and perform database operations using Java objects.

**Importance:** JPA simplifies database access and eliminates the need for writing low-level JDBC code. It promotes a consistent and standardized approach to database management in Java applications.

**Use cases:** JPA is used in Java applications to perform database operations using Java objects and annotations. It is commonly used for building data-driven applications and handling complex database interactions.

### 300: Connecting to the Database in Spring JPA:

**Definition:** To connect to the database in Spring JPA, you need to configure the data source properties in the application's configuration file (e.g., application.properties or application.yml). Spring Boot auto-configures the data source based on the provided properties.

**Importance:** Connecting to the database is a fundamental step in Spring JPA, as it enables the application to interact with the underlying database. Properly configuring the data source ensures that the application can perform database operations successfully.

**Use cases:** Connecting to the database is a prerequisite for using JPA and JPA Repository in Spring applications. It is necessary to store and retrieve data from the database in a Spring JPA-based project.

### 400: Query Methods:

**Definition:** Query Methods in Spring Data JPA are methods defined in a JPA Repository interface that follow a specific naming convention. These methods allow you to define database queries based on method names, eliminating the need for writing custom SQL queries.

**Importance:** Query Methods simplify database querying by providing a way to create dynamic queries using method names. They help in building complex queries based on entity attributes without the need for writing SQL.

**Use cases:** Query Methods are used to define common and custom queries in JPA Repository interfaces. They are commonly used for retrieving data based on various conditions, sorting, and filtering in Spring Data JPA applications.

### 500: @Transactional:

**Definition:** @Transactional is an annotation in Spring that is used to define the transactional behavior of methods or classes. When applied, it ensures that the annotated methods are executed within a transactional context, where either all operations are committed together, or none of them are committed.

**Importance:** @Transactional ensures data consistency and integrity by managing transactions for database operations. It helps in preventing data corruption and maintaining the ACID (Atomicity, Consistency, Isolation, Durability) properties of transactions.

**Use cases:** @Transactional is used in Spring applications to define transactional boundaries around methods or classes that interact with the database. It is commonly used in service layer classes, where multiple database operations need to be executed atomically.
</details>
