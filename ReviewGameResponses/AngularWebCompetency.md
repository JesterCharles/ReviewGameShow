# Angular Web Competency

<details>
<summary> HTML</summary>

### 100: Tags in HTML:

**Definition:** Tags in HTML are markup elements used to define the structure and content of a web page. They consist of an opening tag, content, and a closing tag. Tags are used to create headings, paragraphs, lists, images, links, and other elements on a web page.

**Importance:** Tags are the building blocks of HTML documents. They define the structure and presentation of web content, allowing browsers to render the content appropriately.

**Use cases:** Tags are used whenever you want to structure and format the content of a web page. They are used for headings, paragraphs, tables, forms, and other elements to create a visually appealing and organized web page.

### 200: Forms in HTML:

**Definition:** Forms in HTML are elements used to collect user input. They allow users to submit data to a server for processing. Forms typically include input fields, checkboxes, radio buttons, buttons, and more.

**Importance:** Forms enable user interaction and data submission on web pages. They are essential for building interactive web applications, user registration, login forms, search functionality, and more.

**Use cases:** Forms are used whenever you need to collect user input or allow users to interact with your web application. Common use cases include login forms, registration forms, search bars, feedback forms, and contact forms.

### 300: div in HTML:

**Definition:** The div (division) is a generic container element in HTML used to group and style other elements or content. It is a block-level element that doesn't have any semantic meaning of its own.

**Importance:** div is important for creating layout structures and applying CSS styles to groups of elements. It helps in organizing content on a web page and providing structure to the design.

**Use cases:** div is used whenever you want to group elements together for styling or layout purposes. It is often used as a wrapper to apply styles or structure sections of a web page.

### 400: Semantic Element in HTML:

**Definition:** Semantic elements in HTML provide meaning and context to the content they enclose. Unlike generic elements like div, semantic elements have a specific purpose and convey the role of the content they contain.

**Importance:** Semantic elements enhance web page accessibility, search engine optimization (SEO), and readability for both users and machines. They provide clearer meaning and improve the overall structure of the document.

**Use cases:** Semantic elements are used when you want to provide meaning to the content of a web page. Examples include <header> for the page header, <nav> for navigation links, <main> for the main content, <article> for individual articles, and <footer> for the page footer.

### 500: DOM in HTML:

**Definition:** The DOM (Document Object Model) in HTML is a programming interface that represents the structure of an HTML document as a tree-like data structure. It allows programs to access and manipulate the content and structure of an HTML document dynamically.

**Importance:** The DOM is crucial for dynamic web development as it enables JavaScript to interact with and modify the content of a web page in real-time. It facilitates the creation of interactive and responsive web applications.

**Use cases:** The DOM is used whenever you need to change the content, structure, or style of a web page dynamically based on user interactions or other events. JavaScript libraries and frameworks often rely on the DOM to enable interactive web experiences.
</details>

<details>
<summary>CSS</summary>

### 100: CSS:

**Definition:** CSS (Cascading Style Sheets) is a style sheet language used to describe the presentation and appearance of HTML documents. It allows developers to apply styles, such as colors, fonts, spacing, and layout, to HTML elements, making web pages visually appealing.

**Importance:** CSS is essential for web development as it separates the content (HTML) from its presentation (styles). It enables consistent styling across web pages, improves user experience, and enhances the overall design of websites.

**Use cases:** CSS is used whenever you want to customize the look and feel of web pages. It is used for designing layouts, applying colors and fonts, adding animations, and making responsive designs.

### 200: Internal Styling:

**Definition:** Internal styling in CSS is a method of including CSS code directly within an HTML document using the `style` element in the `head section. The CSS rules defined inside style tags apply only to that specific HTML document.

**Importance:** Internal styling is useful for small web pages with specific styling requirements. It simplifies the process of styling a single HTML page without the need for an external CSS file.

**Use cases:** Internal styling is used when you want to style a single HTML document without creating a separate CSS file. It is commonly used in simple web pages or email templates.

### 300: CSS Box Model:

**Definition:** The CSS Box Model is a concept that describes how elements in CSS are rendered as rectangular boxes. It consists of content, padding, border, and margin, forming a hierarchical structure around the element's content.

**Importance:** Understanding the Box Model is crucial for designing and positioning elements on a web page accurately. It helps in managing spacing, borders, and layout of elements effectively.

**Use cases:** The CSS Box Model is used whenever you need to control the size and spacing of elements on a web page. It is used to create padding around content, add borders, and control the space between elements.

### 400: CSS Selectors:

**Definition:** CSS Selectors are patterns used to select and target specific HTML elements for applying styles. Selectors allow developers to specify which elements should receive the defined styles.

**Importance:** CSS Selectors play a central role in applying styles to targeted elements. They provide flexibility and granularity in styling specific elements or groups of elements.

**Use cases:** CSS Selectors are used in CSS rules to define which elements should receive the specified styles. They are used to apply styles to headings, links, lists, tables, form elements, and more.

### 500: Responsive Web Design:

**Definition:** Responsive Web Design is an approach to web development that aims to create web pages that adapt and respond to different devices and screen sizes. It ensures optimal user experience across desktops, tablets, and smartphones.

**Importance:** Responsive Web Design is crucial in the era of diverse devices with varying screen sizes. It improves accessibility, user engagement, and search engine rankings. It eliminates the need for creating separate mobile versions of a website.

**Use cases:** Responsive Web Design is used when you want to build websites that work seamlessly on various devices. It is used to create fluid layouts, use media queries, and optimize images to enhance the user experience on different screen sizes.
</details>

<details>
<summary>JavaScript</summary>

### 100: JS Data Types:

**Definition:** JavaScript has several data types, including primitive data types such as number, string, boolean, null, undefined, bigint, and symbol, and reference data types like object and array. Data types define the kind of data that can be stored and manipulated in JavaScript.

**Importance:** Understanding JavaScript data types is crucial for working with variables, performing operations, and passing values between functions. It helps prevent unexpected behavior and ensures correct data manipulation.

**Use cases:** JavaScript data types are used in variable declarations, function arguments, and data manipulation operations. For example, you use number data type for mathematical calculations, strings for text manipulation, booleans for conditional checks, and objects for organizing complex data structures.

### 200: let and const keywords:

**Definition:** `let` and `const` are block-scoped variable declarations introduced in ES6 (ECMAScript 2015). `let` allows you to declare variables that can be reassigned, while `const` is used for declaring variables with constant values that cannot be reassigned.

**Importance:** `let` and `const` help in creating block-scoped variables, reducing the risk of variable name conflicts and improving code maintainability. `const` ensures that the value of a variable remains constant, preventing accidental reassignment.

**Use cases:** `let` is used when you need to declare variables that may change their values during the program execution. `const` is used when you want to define variables with constant values, like configuration settings, mathematical constants, or constants in the application logic.

### 300: Arrow Notation:

**Definition:** Arrow notation, also known as arrow functions, is a concise syntax introduced in ES6 for defining functions in JavaScript. It provides a shorter and more readable way of writing function expressions.

**Importance:** Arrow notation simplifies the syntax for writing small functions, making the code more concise and easier to understand. It also provides lexical scoping for `this`, ensuring predictable behavior when working with objects and functions.

**Use cases:** Arrow notation is used when you need to define short, one-line functions or callback functions, especially in functional programming and event handling. It helps reduce boilerplate code and enhances the readability of the codebase.

### 400: Higher Order Functions:

**Definition:** Higher Order Functions (HOFs) are functions that take one or more functions as arguments or return another function as their result. They enable functional programming paradigms and are a powerful feature in JavaScript.

**Importance:** Higher Order Functions allow developers to write more modular and reusable code. They promote a functional programming style, enhancing code readability and reducing side effects.

**Use cases:** Higher Order Functions are used when you need to perform operations on functions, create function compositions, implement callbacks, and apply functional programming principles like map, filter, reduce, and forEach on arrays and collections.

### 500: Promises:

**Definition:** Promises are a feature introduced in ES6 for handling asynchronous operations in JavaScript. A promise represents a value that may not be available yet, but will be resolved (fulfilled) or rejected with a reason.

**Importance:** Promises simplify asynchronous programming, making it easier to manage and reason about asynchronous tasks. They provide a clean and structured way to handle success and failure scenarios of asynchronous operations.

**Use cases:** Promises are used for API requests, file reading/writing, and database queries. They are commonly used in modern JavaScript applications to avoid callback hell and improve code readability.
</details>

<details>
<summary>TypeScript</summary>

### 100: TypeScript:

**Definition:** TypeScript is a superset of JavaScript developed by Microsoft. It adds optional static typing, interfaces, classes, and other features to JavaScript. TypeScript code is transpiled into plain JavaScript, making it compatible with all modern browsers and JavaScript runtimes.

**Importance:** TypeScript enhances JavaScript development by providing static type checking, enabling better code organization, improved tooling support, and enhanced code maintainability. It helps catch errors early in the development process, reducing bugs and improving code quality.

**Use cases:** TypeScript is used in projects where developers want the benefits of static typing and enhanced tooling while still targeting JavaScript. It is popular in large-scale applications, frameworks, and projects with large development teams.

### 200: Interfaces with TypeScript:

**Definition:** Interfaces in TypeScript define a contract for objects, specifying the structure and types of properties or methods that must be present in an implementing object. They provide a way to describe the shape of objects and enforce consistency.

**Importance:** Interfaces promote strong typing and better code organization by enabling developers to define clear and consistent object structures. They help catch type-related errors early and improve code maintainability.

**Use cases:** Interfaces are used when you want to create object blueprints that define the properties and methods required for an object to fulfill a specific role or contract. They are commonly used to define data structures, APIs, and class implementation expectations.

### 300: Access Modifiers in TypeScript:

**Definition:** Access modifiers in TypeScript (public, private, and protected) determine the visibility and accessibility of class members (properties and methods). They control how the class members can be accessed and modified from outside the class.

**Importance:** Access modifiers help enforce encapsulation and control the level of abstraction in a class. They provide security by restricting access to sensitive data and promote a clear separation of concerns.

**Use cases:** Access modifiers are used when you want to control the visibility and accessibility of class members. `public` allows unrestricted access, `private` restricts access to the class itself, and `protected` allows access within the class and its subclasses.

### 400: Decorators:

**Definition:** Decorators are a feature in TypeScript used to modify classes, methods, properties, or parameters. They are indicated by the `@` symbol followed by the decorator name and are applied using the decorator design pattern.

**Importance:** Decorators provide a way to extend and modify the behavior of classes and their members without altering their core implementation. They enable aspects like logging, validation, dependency injection, and more.

**Use cases:** Decorators are used when you want to add functionalities or metadata to classes, methods, or properties. They are commonly used in frameworks like Angular and NestJS for dependency injection, routing, and custom annotations.

### 500: Enums:

**Definition:** Enums in TypeScript are a feature that allows developers to define a set of named constants. Enums provide a way to represent a group of related values with readable names, making code more self-descriptive.

**Importance:** Enums improve code readability and maintainability by giving meaningful names to numeric or string values. They help avoid magic numbers and string literals in the code.

**Use cases:** Enums are used when you want to represent a fixed set of related values. They are commonly used for representing days of the week, error codes, status states, and other sets of related constants.
</details>

<details>
<summary>Angular</summary>

### 100: SPA:

**Definition:** SPA (Single Page Application) is a web application architecture that loads a single HTML page and dynamically updates its content as the user interacts with the application. SPAs use JavaScript frameworks to handle client-side routing and data manipulation, providing a seamless user experience.

**Importance:** SPAs offer a more fluid user experience compared to traditional multi-page applications. They reduce page reloads, improve performance, and allow developers to build interactive and responsive applications.

**Use cases:** SPAs are used when you want to create web applications that behave like desktop applications. They are commonly used in modern web development to build complex and interactive applications, such as social media platforms, productivity tools, and e-commerce websites.

### 200: Angular CLI:

**Definition:** Angular CLI (Command Line Interface) is a command-line tool provided by Angular that simplifies and automates various tasks in Angular development. It includes features like project scaffolding, code generation, testing, and building applications.

**Importance:** Angular CLI streamlines the Angular development process, reducing manual configuration and boilerplate code. It ensures consistent project structure and provides a set of best practices to follow.

**Use cases:** Angular CLI is used to create new Angular projects, generate components, services, modules, and run development servers. It is an essential tool for Angular developers to improve productivity and maintain project consistency.

### 300: @NgModule:

**Definition:** @NgModule is a decorator in Angular used to define a module. An Angular module is a container that organizes related components, directives, services, and other assets into cohesive units.

**Importance:** @NgModule helps in modularizing and organizing Angular applications. It provides a way to encapsulate functionality, manage dependencies, and improve application performance by enabling lazy loading.

**Use cases:** @NgModule is used when you want to create reusable and self-contained units of an Angular application. It is commonly used to group related components, services, and directives into feature modules for better code organization.

### 400: Data Binding:

**Definition:** Data Binding is a feature in Angular that establishes a connection between the application's data and the user interface. It allows automatic synchronization of data changes between the model (data) and the view (UI).

**Importance:** Data Binding simplifies the process of updating the UI when the underlying data changes, reducing the need for manual DOM manipulation. It provides a declarative way to manage data and ensure consistency across the application.

**Use cases:** Data Binding is used to display and update data in the user interface. It is commonly used in form elements, displaying real-time data, and implementing two-way data binding to synchronize changes between model and view.

### 500: Directives:

**Definition:** Directives are a feature in Angular that extend the behavior of HTML elements. They allow developers to attach custom behaviors to elements or manipulate the DOM.

**Importance:** Directives enable code reusability and enhance the functionality of HTML elements. They provide a way to encapsulate complex UI interactions and enable the creation of custom components and structural changes to the DOM.

**Use cases:** Directives are used to create reusable components, add event handling, apply CSS styling dynamically, and manipulate the DOM. They are commonly used to implement custom input validation, create tooltips, handle user interactions, and add custom behavior to elements.
</details>

<details>
<summary>Angular Advanced</summary>

### 100: Pipes in Angular:

**Definition:** Pipes in Angular are a feature that allows you to transform and format data in the template before displaying it to the user. They are used to apply filters, convert data types, and perform other operations on data.

**Importance:** Pipes enhance the user experience by providing a convenient way to format data in the template without modifying the underlying data in the component. They promote code reusability and maintainability by encapsulating data transformation logic.

**Use cases:** Pipes are used whenever you need to format and display data in a specific way in the template. Common use cases include formatting dates, currency, numbers, converting text to uppercase or lowercase, and filtering arrays.

### 200: Service in Angular:

**Definition:** A Service in Angular is a class that provides functionality and data that can be shared across different components and modules. It acts as a central place for business logic, data manipulation, and communication with external services.

**Importance:** Services promote the principle of separation of concerns and help in maintaining clean and modular code. They enable code reuse, dependency injection, and the centralization of data and logic.

**Use cases:** Services are used when you want to share data, perform HTTP requests, handle business logic, and interact with external APIs or databases. They are commonly used to manage user authentication, handle data retrieval, and perform other application-specific tasks.

### 300: HttpClient:

**Definition:** HttpClient is a service in Angular that allows you to make HTTP requests to interact with servers and external APIs. It provides methods for performing GET, POST, PUT, DELETE, and other HTTP operations.

**Importance:** HttpClient simplifies the process of making HTTP requests and handling responses. It supports features like request headers, query parameters, error handling, and response transformations.

**Use cases:** HttpClient is used whenever you need to send HTTP requests and receive responses in Angular applications. It is commonly used for fetching data from RESTful APIs, submitting form data, and interacting with external web services.

### 400: Routing with Angular:

**Definition:** Routing in Angular is a mechanism that allows you to navigate between different components and views within a single-page application. It uses the Angular Router module to handle URL-based navigation and view rendering.

**Importance:** Routing provides a seamless user experience by enabling navigation without page reloads. It helps in building complex applications with multiple views and organizing the application's structure.

**Use cases:** Routing is used when you want to create a multi-page-like experience in a single-page application. It is commonly used for building navigation menus, implementing user authentication, and organizing content in different views.

### 500: Route Guards:

**Definition:** Route Guards in Angular are a feature that allows you to control access to routes based on certain conditions. They are used to protect routes from unauthorized access, validate user permissions, and perform other checks before navigation.

**Importance:** Route Guards enhance security and user experience by preventing unauthorized access to routes and ensuring that the user meets specific criteria before navigating to a route.

**Use cases:** Route Guards are used when you want to control access to specific routes in an Angular application. They are commonly used for implementing authentication checks, role-based access control, and handling redirects based on certain conditions.
</details>