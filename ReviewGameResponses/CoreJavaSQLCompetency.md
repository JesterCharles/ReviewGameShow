# Core Java/SQL Competency

<details>
<summary>Java</summary>

### 100: For-each loop in Java:

**Definition:** A for-each loop (also known as an enhanced for loop) in Java is a simplified loop construct that allows you to iterate over elements in an array or a collection without the need for explicit indexing or iteration controls.

**Importance:** The for-each loop enhances code readability and reduces the chances of errors related to indexing or off-by-one errors when iterating over collections.

**Use cases:** It is commonly used when you want to process each element in an array or collection sequentially, without having to manage the loop index manually.

### 200: Checked and unchecked exceptions in Java:

**Definition:** In Java, exceptions are divided into two types: checked exceptions and unchecked exceptions. Checked exceptions are those that the compiler forces the programmer to handle explicitly, either by using a `try-catch` block or declaring the exception in the method's signature using the `throws` keyword. Unchecked exceptions, on the other hand, do not require explicit handling.

**Importance:** The distinction between checked and unchecked exceptions helps in writing more robust and maintainable code. Checked exceptions ensure that certain exceptional situations are handled gracefully, while unchecked exceptions are typically used for programming errors and unexpected situations.

**Use cases:** Checked exceptions are often used for situations where recovery is possible and expected, such as file I/O, network operations, and database interactions. Unchecked exceptions are used for scenarios like division by zero, array index out of bounds, and null pointer references, which are indicative of programming errors and should be corrected during development.

### 300: Abstract class in Java:

**Definition:** An abstract class in Java is a class that cannot be instantiated directly, meaning you cannot create objects of the abstract class. It serves as a blueprint for other classes and can contain both abstract and concrete methods.

**Importance:** Abstract classes provide a way to define common behavior and structure among related classes while leaving specific implementation details to the subclasses. They facilitate code reusability and help establish a hierarchy among related classes.

**Use cases:** Abstract classes are used when you want to create a base class that contains some default behavior or functionality that should be implemented by its subclasses. They are commonly employed in class hierarchies and frameworks.

### 400: Overriding a static method in Java:

**Definition:** In Java, you cannot override a static method. Instead, you can only hide the static method by declaring another static method with the same name in the subclass. The choice of which method to invoke is determined at compile-time based on the reference type.

**Importance:** Overriding is based on dynamic binding, where the actual method to be executed is determined at runtime based on the object's type. However, since static methods are associated with the class rather than instances, dynamic binding doesn't apply to static methods.

**Use cases:** When you have a static method in the superclass and want to provide a different implementation in the subclass, you can declare another static method with the same name in the subclass. Keep in mind that this will not override the superclass's static method but will only hide it.

### 500: Equals() and hashCode() methods in Java:

**Definition:** In Java, `equals()` is a method used to compare the content or value equality of objects, while `hashCode()` is a method that returns a hash code value for an object, which is used in hash-based data structures like HashMap, HashSet, etc.

**Importance:** When using hash-based data structures, it's crucial to ensure that the `hashCode()` method is consistent with the `equals()` method. Otherwise, you may encounter unexpected behavior and difficulties in retrieving objects from collections.

**Use cases:** When you want to store objects in hash-based data structures, you should override both `equals()` and `hashCode()` methods to provide correct and consistent behavior for object comparison and retrieval operations. Failing to do so might lead to issues like duplicate entries in sets or maps and inability to retrieve objects as expected.
</details>

<details>
<summary>DS&A</summary>

### 100: Algorithm in Java:

**Definition:** An algorithm in Java (or any programming language) is a step-by-step procedure or set of instructions to solve a specific problem or perform a particular task. It is a well-defined sequence of actions that provides a clear solution to the given problem.

**Importance:** Algorithms are fundamental in computer programming as they enable developers to create efficient, reliable, and optimized solutions to various computational problems. Understanding algorithms helps in developing better code and optimizing performance.

**Use cases:** Algorithms are used in various applications, such as searching, sorting, graph traversal, pattern matching, and data manipulation. They are essential in solving complex problems in fields like data analysis, artificial intelligence, and cryptography.

### 200: Time Complexity:

**Definition:** Time complexity in Java (and other programming languages) refers to the analysis of the running time of an algorithm with respect to the size of the input. It quantifies the amount of time an algorithm takes to execute in terms of the input size.

**Importance:** Time complexity is crucial for evaluating the efficiency of algorithms. It allows programmers to compare different algorithms and choose the most suitable one for a given problem based on how it scales with input size.

**Use cases:** Time complexity analysis is used in algorithm design, optimization, and selecting appropriate data structures. It helps in identifying potential performance bottlenecks and improving the overall efficiency of programs.

### 300: Bubble Sort:

**Definition:** Bubble Sort is a simple sorting algorithm in Java that repeatedly steps through the list of elements to be sorted, compares adjacent elements, and swaps them if they are in the wrong order. The process is repeated until the entire list is sorted.

**Importance:** Bubble Sort is easy to understand and implement, making it useful for educational purposes and small lists of elements. However, it is not efficient for large datasets due to its quadratic time complexity.

**Use cases:** Bubble Sort can be used when the list to be sorted is small, and simplicity of the algorithm outweighs its inefficiency. However, for real-world applications, more efficient sorting algorithms like QuickSort or MergeSort are preferred.

### 400: Linear Search:

**Definition:** Linear Search, also known as sequential search, is a searching algorithm in Java that traverses a list of elements one by one to find a specific target element. It compares each element sequentially until a match is found or the entire list is searched.

**Importance:** Linear Search is straightforward to implement and works on unsorted as well as sorted lists. However, it becomes inefficient for large datasets as it has a linear time complexity.

**Use cases:** Linear Search is suitable for small lists or when the list is not sorted. It is often used as a fallback option when the list is not too large and efficient searching algorithms like Binary Search are not applicable.

### 500: LinkedList:

**Definition:** LinkedList is a linear data structure in Java that consists of a sequence of elements, known as nodes, where each node contains data and a reference (or pointer) to the next node in the sequence.

**Importance:** LinkedLists provide dynamic memory allocation and efficient element insertion and deletion compared to arrays. They are useful when the size of the data is unknown or needs to be frequently modified during program execution.

**Use cases:** LinkedLists are used in various scenarios, such as implementing stacks, queues, and other data structures. They are also used in certain graph algorithms and provide the foundation for more advanced data structures like doubly linked lists and circular linked lists.
</details>

<details>
<summary>Java 8 Features</summary>

### 100: Lambdas in Java 8:

**Definition:** Lambdas in Java 8 are a concise way to represent anonymous functions, also known as lambda expressions. They allow you to treat functions as method arguments or code as data. Lambdas facilitate functional programming by enabling a functional style of coding in Java.

**Importance:** Lambdas make it easier to write more readable and concise code, especially when dealing with functional interfaces like Runnable, Callable, Comparator, etc. They promote functional programming paradigms and are essential for utilizing the Stream API effectively.

**Use cases:** Lambdas are commonly used in Java 8 and later versions for implementing functional interfaces in a more compact and expressive manner. They are widely used in scenarios where you need to pass behavior as an argument to a method or when working with collections and the Stream API.

### 200: Optional Class:

**Definition:** The Optional class in Java is a container object that may or may not contain a non-null value. It is introduced to handle scenarios where a method might return a null value, avoiding potential NullPointerExceptions.

**Importance:** Optional helps in writing more robust and less error-prone code. It forces developers to handle the possibility of a value being absent explicitly, reducing the chances of null-related runtime exceptions.

**Use cases:** Optional is useful in methods where the result might be absent under certain conditions. It is often used for return types to indicate that a method can return a value, but that value might be null in some cases.

### 300: Reflection API:

**Definition:** The Reflection API in Java allows the examination and manipulation of classes, methods, fields, and interfaces at runtime. It enables the dynamic inspection of Java classes and their members.

**Importance:** Reflection is crucial for various advanced Java applications, such as building tools like IDEs and profilers. It facilitates frameworks that rely on runtime introspection to provide generic solutions without knowing the class structures at compile time.

**Use cases:** Reflection is used in scenarios where you need to analyze and manipulate Java classes and objects at runtime, e.g., serialization, dependency injection, testing frameworks, and creating generic libraries.

### 400: Method Reference:

**Definition:** Method reference in Java is a shorthand syntax for representing lambda expressions. It allows you to reference existing methods or constructors and use them as lambda expressions instead of explicitly providing a full lambda body.

**Importance:** Method references improve code readability and maintainability, especially when the lambda expression merely calls an existing method or constructor. They provide a more concise and natural way to express functionality.

**Use cases:** Method references are used when you have lambda expressions that do nothing more than call an existing method. They can be particularly helpful when working with the Stream API, functional interfaces, and other functional programming constructs.

### 500: Stream API:

**Definition:** The Stream API in Java is a new feature introduced in Java 8 that provides a sequence of elements and supports functional-style operations on those elements. It enables declarative and parallel processing of data collections.

**Importance:** The Stream API simplifies and optimizes data processing tasks, making them more readable and efficient. It encourages functional programming, which leads to more concise and expressive code.

**Use cases:** The Stream API is widely used for processing collections of data in various scenarios, such as filtering, mapping, reducing, and parallel processing. It is extensively used for manipulating and transforming data in a functional and declarative manner.
</details>

<details>
<summary>Threads</summary>

### 100: Thread Class:

**Definition:** The Thread class in Java represents a thread of execution within a program. It is a part of the Java Multithreading API and provides methods to create, manage, and control threads in a Java application.

**Importance:** Threads allow a Java program to perform multiple tasks concurrently, improving performance and responsiveness. The Thread class provides essential functionalities to work with threads, such as creating new threads, starting them, pausing, resuming, and terminating them.

**Use cases:** The Thread class is used when you want to perform multiple tasks simultaneously and independently in a Java program. It is commonly employed in scenarios where parallel processing or handling concurrent tasks is necessary.

### 200: Runnable Interface:

**Definition:** The Runnable interface in Java is a functional interface that represents a task that can be executed concurrently by a thread. It provides a single abstract method `run()`, which is responsible for defining the task's behavior.

**Importance:** The Runnable interface decouples the task's implementation from the thread management, promoting better separation of concerns and code reusability. It serves as an alternative to directly extending the Thread class for creating threads.

**Use cases:** The Runnable interface is used when you want to define a task that can be executed concurrently by multiple threads. It is commonly employed to implement worker threads, parallel processing, and concurrent tasks.

### 300: Multi-threading:

**Definition:** Multi-threading in Java refers to the concurrent execution of multiple threads within the same Java application. Each thread represents an independent flow of control, allowing the program to perform several tasks simultaneously.

**Importance:** Multi-threading is essential for improving the efficiency and responsiveness of Java applications. It maximizes CPU utilization, allows for better resource management, and enables the handling of time-consuming operations without blocking the main thread.

**Use cases:** Multi-threading is used in various scenarios, such as performing time-consuming computations in the background, handling multiple client requests in server applications, and implementing user interfaces with responsive behavior while performing tasks in the background.

### 400: 'synchronized' keyword:

**Definition:** The 'synchronized' keyword in Java is used to create synchronized blocks or methods that provide mutually exclusive access to critical sections of code. It ensures that only one thread can execute the synchronized code at a time, preventing race conditions and thread interference.

**Importance:** Synchronization is crucial for maintaining data consistency and avoiding thread-related issues like data corruption or unpredictable behavior due to concurrent access.

**Use cases:** The 'synchronized' keyword is used when multiple threads need access to shared resources or critical sections that should not be accessed concurrently. It is commonly used to protect access to shared variables, avoiding potential data race conditions.

### 500: Deadlock:

**Definition:** Deadlock is a situation in concurrent programming where two or more threads are unable to proceed further because each thread is waiting for a resource that is held by another thread, creating a circular dependency and a standstill in program execution.

**Importance:** Deadlocks are critical issues in multi-threaded applications as they can lead to program freezes and unresponsiveness. Detecting and resolving deadlocks is essential for maintaining the stability and correct behavior of concurrent programs.

**Use cases:** Deadlocks can occur in multi-threaded applications where multiple threads contend for shared resources, such as locks, files, or network connections. Avoiding deadlocks requires careful design and proper synchronization techniques.
</details>

<details>
<summary>SQL</summary>

### 100: Table in SQL:

**Definition:** In SQL, a table is a structured collection of data organized into rows and columns. It represents a logical structure that stores data in a tabular format, where each row represents a record, and each column represents a data attribute.

**Importance:** Tables are fundamental components of a relational database management system (RDBMS). They provide a structured way to store and manage data, allowing efficient data retrieval, manipulation, and organization.

**Use cases:** Tables are used to store various types of data, such as user information, product details, sales records, and much more. They form the foundation of a database and play a crucial role in building data-driven applications.

### 200: ORDER BY clause in SQL:

**Definition:** The ORDER BY clause in SQL is used to sort the result set of a query based on one or more specified columns. It arranges the rows in ascending or descending order according to the values in the specified columns.

**Importance:** The ORDER BY clause is essential for organizing query results in a meaningful way. It allows data to be presented in a specific order, making it easier for users to interpret and analyze the data.

**Use cases:** The ORDER BY clause is used whenever the result set needs to be sorted for presentation purposes or to apply a particular order to the data for further processing.

### 300: Constraints in SQL:

**Definition:** Constraints in SQL are rules applied to the columns or tables to maintain data integrity and ensure data validity. They define limitations and conditions that data must adhere to, preventing the insertion of inconsistent or incorrect data.

**Importance:** Constraints play a critical role in maintaining data integrity and preventing data corruption or inconsistency. They enforce business rules and ensure that the data meets specific requirements.

**Use cases:** Constraints are used to enforce various conditions, such as primary key constraints to enforce uniqueness, foreign key constraints to maintain referential integrity, check constraints to limit valid values, and not-null constraints to ensure that a column cannot have a null value.

### 400: WHERE clause in SQL:

**Definition:** The WHERE clause in SQL is used to filter the rows returned by a SELECT, UPDATE, or DELETE statement. It specifies a condition that must be satisfied by the rows to be included in the result set.

**Importance:** The WHERE clause allows you to extract specific data from a table based on specific criteria. It provides flexibility in querying and enables you to retrieve only the data you need.

**Use cases:** The WHERE clause is commonly used in SELECT statements to filter data based on specific conditions. It is helpful for extracting relevant information from large datasets and performing data analysis.

### 500: Stored Procedure in SQL:

**Definition:** A stored procedure in SQL is a precompiled and stored set of SQL statements that can be executed as a single unit. It is stored within the database and can be called and executed multiple times from various client applications.

**Importance:** Stored procedures offer several benefits, including improved performance due to precompilation, code reusability, security, and encapsulation of complex logic within the database.

**Use cases:** Stored procedures are used for performing complex operations that involve multiple SQL statements, business logic, or data validation. They are commonly used in web applications, enterprise systems, and data-driven applications where efficient data manipulation and processing are required.
</details>

<details>
<summary>JDBC</summary>

### 100: JDBC API:

**Definition:** JDBC (Java Database Connectivity) API is a Java API that provides a standard way to interact with relational databases. It allows Java applications to connect to and manipulate databases using SQL queries and statements.

**Importance:** The JDBC API is essential for developing database-driven applications in Java. It enables seamless communication between Java code and databases, making it possible to store, retrieve, and manipulate data efficiently.

**Use cases:** The JDBC API is used whenever a Java application needs to interact with a relational database. It is commonly used in web applications, enterprise software, and any other system that requires database access.

### 200: DriverManager:

**Definition:** The DriverManager class in JDBC is a part of the Java Standard API that manages the set of registered JDBC drivers. It is responsible for establishing and maintaining database connections using the appropriate driver.

**Importance:** The DriverManager is a crucial component in the JDBC API as it facilitates the process of connecting to databases using different JDBC drivers. It simplifies the process of managing and selecting the appropriate driver for the database connection.

**Use cases:** Developers use the DriverManager class to obtain a connection to a specific database by providing the necessary connection details and credentials. This class is typically used at the beginning of a Java application to establish a connection with the database.

### 300: Connection:

**Definition:** Connection in JDBC represents a session with a specific database. It allows the Java application to send SQL statements to the database and receive results. The Connection object also encapsulates transaction management and connection-related properties.

**Importance:** The Connection object is essential for performing various database operations in Java. It allows the application to interact with the database, execute SQL queries, and commit or rollback transactions.

**Use cases:** The Connection object is used throughout a Java application to perform database operations like querying data, inserting, updating, and deleting records, managing transactions, and handling database connections efficiently.

### 400: PreparedStatement:

**Definition:** PreparedStatement in JDBC is an interface that extends the Statement interface. It represents a precompiled SQL statement that can be executed multiple times with different parameters. It is used to execute parameterized queries, improving performance and security.

**Importance:** PreparedStatement is crucial for optimizing the execution of similar SQL statements with different parameter values. It allows the database to prepare and cache the SQL query, leading to better performance and protection against SQL injection attacks.

**Use cases:** PreparedStatement is used when you need to execute the same SQL query multiple times with different parameter values. It is commonly used for queries that involve user input or dynamic values.

### 500: CallableStatement:

**Definition:** CallableStatement in JDBC is an interface that extends the PreparedStatement interface. It is used to call stored procedures or functions in the database. It allows the execution of database-specific procedural calls.

**Importance:** CallableStatement is essential for invoking database procedures and functions from a Java application. It provides a standard way to interact with stored procedures and retrieve their output.

**Use cases:** CallableStatement is used when you want to execute stored procedures or functions in the database. It is commonly used in enterprise applications that rely on stored procedures for complex database operations.

</details>
