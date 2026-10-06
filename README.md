# NestJS Interview Questions & Answers

> Welcome to the NestJS Interview Questions and Answers repository!

- This repository aims to be a comprehensive resource for NestJS developers preparing for interviews. Whether you're a beginner or an experienced developer, this collection of questions and answers is designed to help you brush up on your NestJS knowledge and excel in interviews.
  > Click ⭐if you like the project and incase you're interested in contributing to this project. Before you dive in, please take a moment to review our guidelines.

## Important Links

- [Code of Conduct](./CODE_OF_CONDUCT.md): I expect everyone participating in this project to follow the code of conduct. Make sure you understand and adhere to these guidelines.

- [Contributing Guidelines](./CONTRIBUTING.md): Before contributing, please read the contributing guidelines. They provide information on how to submit questions, report issues, and more.

> Follow me [@himanshudevgupta](https://github.com/himanshudevgupta).

### Table of Contents

| No. | Questions                                                                                                                                                                                                                                                                                                                                                                                                |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [What is Nestjs?](#what-is-nestjs)                                                                                                                                                                                                                                                                                                                                                                       |
| 2   | [Who developed NestJS? Why did they develop NestJS?](#who-developed-nestjs-why-did-they-develop-nestjs)                                                                                                                                                                                                                                                                                                  |
| 3   | [When was NestJS first released?](#when-was-nestjs-first-released)                                                                                                                                                                                                                                                                                                                                       |
| 4   | [How can you install NestJS and set up a new project on your machine?](#how-can-you-install-nestjs-and-set-up-a-new-project-on-your-machine)                                                                                                                                                                                                                                                             |
| 5   | [What’s the difference between NestJS and Angular?](#what-s-the-difference-between-nestjs-and-angular?)                                                                                                                                                                                                                                                                                                  |
| 6   | [Is it possible to use other languages like C++, Ruby or Python with NestJS? If yes, then how?](#is-it-possible-to-use-other-languages-like-c-ruby-or-python-with-nestjs-if-yes-then-how)                                                                                                                                                                                                                |
| 7   | [What are the main components of a NestJS application?](#what-are-the-main-components-of-a-nestjs-application)                                                                                                                                                                                                                                                                                           |
| 8   | [How to declare a class as a controller in Nest.js](#how-to-declare-a-class-as-a-controller-in-nestjs)                                                                                                                                                                                                                                                                                                   |
| 9   | [Can you explain how to use decorators in a NestJS controller?](#can-you-explain-how-to-use-decorators-in-a-nestjs-controller)                                                                                                                                                                                                                                                                           |
| 10  | [How can you use route parameters in a NestJS controller?](#how-can-you-use-route-parameters-in-a-nestjs-controller)                                                                                                                                                                                                                                                                                     |
| 11  | [What is the role of the `@Body()` decorator?](#what-is-the-role-of-the-body-decorator)                                                                                                                                                                                                                                                                                                                  |
| 12  | [What is an interceptor in the context of NestJS?](#what-is-an-interceptor-in-the-context-of-nestjs)                                                                                                                                                                                                                                                                                                     |
| 13  | [What are pipes in the context of NestJS?](#what-are-pipes-in-the-context-of-nestjs)                                                                                                                                                                                                                                                                                                                     |
| 14  | [What are guards in the context of NestJS?](#what-are-guards-in-the-context-of-nestjs)                                                                                                                                                                                                                                                                                                                   |
| 15  | [What are middlewares in the context of NestJS?](#what-are-middlewares-in-the-context-of-nestjs)                                                                                                                                                                                                                                                                                                         |
| 16  | [Explain the concept of Dependency Injection in NestJS. How does it help in building modular and testable applications?](#explain-the-concept-of-dependency-injection-in-nestjs-how-does-it-help-in-building-modular-and-testable-applications)                                                                                                                                                          |
| 17  | [What’s the difference between @injectable() and @inject() decorators?](#what-s-the-difference-between-injectable-and-inject-decorators)                                                                                                                                                                                                                                                                 |
| 18  | [How does the Nest logger differ from the standard console.log() and when would you prefer one over the other?](#how-does-the-nest-logger-differ-from-the-standard-console-log-and-when-would-you-prefer-one-over-the-other)                                                                                                                                                                             |
| 19  | [What is the difference between interceptors and middleware?](#what-is-the-difference-between-interceptors-and-middleware)                                                                                                                                                                                                                                                                               |
| 20  | [What testing frameworks work best with NestJS?](#what-testing-frameworks-work-best-with-nestjs)                                                                                                                                                                                                                                                                                                         |
| 21  | [Explain the purpose of DTOs (Data Transfer Objects) in NestJS.](#explain-the-purpose-of-dtos-data-transfer-objects-in-nestjs.)                                                                                                                                                                                                                                                                          |
| 22  | [How can you handle asynchronous operations in NestJS, and what is the role of the Promise object?](#how-can-you-handle-asynchronous-operations-in-nestjs-and-what-is-the-role-of-the-promise-object)                                                                                                                                                                                                    |
| 23  | [Explain the purpose of the @InjectRepository() decorator in NestJS.](#explain-the-purpose-of-the-injectrepository-decorator-in-nestjs)                                                                                                                                                                                                                                                                  |
| 24  | [Explain the purpose of the @nestjs/jwt package in NestJS?](#explain-the-purpose-of-the-nestjs-jwt-package-in-nestjs)                                                                                                                                                                                                                                                                                    |
| 25  | [Discuss how tokens are used for authorization in an API. What is the difference between authentication and authorization, and how are these processes implemented with tokens?](#discuss-how-tokens-are-used-for-authorization-in-an-api-what-is-the-difference-between-authentication-and-authorization-and-how-are-these-processes-implemented-with-tokens)                                           |
| 26  | [Why is it important for tokens to have an expiration time? How can you implement token expiration in NestJS, and what role do refresh tokens play in maintaining user sessions?](#why-is-it-important-for-tokens-to-have-an-expiration-time-How-can-you-implement-token-expiration-in-nestjs-and-what-role-do-refresh-tokens-play-in-maintaining-user-sessions)                                         |
| 27  | [Describe the mechanism for a token refresh in NestJS. How can you implement an automatic token refresh strategy to maintain user sessions?](#describe-the-mechanism-for-a-token-refresh-in-nestjs-how-can-you-implement-an-automatic-token-refresh-strategy-to-maintain-user-sessions)                                                                                                                  |
| 28  | [How does NestJS support authentication and authorization?](#how-does-nestjs-support-authentication-and-authorization)                                                                                                                                                                                                                                                                                   |
| 29  | [What is the difference between Provider and Services in Nestjs, can we have a provider without an injectable decorator, Give examples?](#what-is-the-difference-between-provider-and-services-in-nestjs-can-we-have-a-provider-without-an-injectable-decorator-give-examples.)                                                                                                                          |
| 30  | [What are custom providers and how do they differ from standard Providers in Nest.js?](#what-are-custom-providers-and-how-do-they-differ-from-standard-providers-in-nestjs)                                                                                                                                                                                                                              |
| 31  | [How can you generate API documentation using Swagger in NestJS? Discuss the importance of documenting your API and how it benefits developers?](#how-can-you-generate-api-documentation-using-swagger-in-nestjs-discuss-the-importance-of-documenting-your-api-and-how-it-benefits-developers)                                                                                                          |
| 32  | [Explain the purpose of the @nestjs/swagger ApiProperty(), ApiOperation() decorators?](#explain-the-purpose-of-the-nestjs-swagger-apiproperty-apioperation-decorators)                                                                                                                                                                                                                                   |
| 33  | [Explain the purpose of the Dockerfile in a NestJS application, and how it facilitates containerization?](#explain-the-purpose-of-the-dockerfile-in-a-nestjs-application-and-how-it-facilitates-containerization)                                                                                                                                                                                        |
| 34  | [How can you use Docker Compose with NestJS, and what is its role in a multi-container setup?](#how-can-you-use-docker-compose-with-nestjs-and-what-is-its-role-in-a-multi-container-setup)                                                                                                                                                                                                              |
| 35  | [What is the purpose of the @nestjs/passport package, and how does it facilitate authentication in NestJS?](#what-is-the-purpose-of-the-nestjs-passport-package-and-how-does-it-facilitate-authentication-in-nestjs)                                                                                                                                                                                     |
| 36  | [How can you handle file uploads in NestJS, and what is the role of the Multer library?](#how-can-you-handle-file-uploads-in-nestjs-and-what-is-the-role-of-the-multer-library)                                                                                                                                                                                                                          |
| 37  | [How does NestJS handle database interactions, and what are the supported databases?](#how-does-nestjs-handle-database-interactions-and-what-are-the-supported-databases)                                                                                                                                                                                                                                |
| 38  | [What is Circular dependency (dependency cycle) in Nestjs, and how can they be fixed?](#what-is-circular-dependency-dependency-cycle-in-nestjs-and-how-can-they-be-fixed)                                                                                                                                                                                                                                |
| 39  | [How can you handle errors in NestJS?](#how-can-you-handle-errors-in-nestjs)                                                                                                                                                                                                                                                                                                                             |
| 40  | [How does NestJS handle CORS (Cross-Origin Resource Sharing)?](#how-does-nestjs-handle-cors-cross-origin-resource-sharing)                                                                                                                                                                                                                                                                               |
| 41  | [Explain the purpose of the ExecutionContext in NestJS Middleware?](#explain-the-purpose-of-the-executioncontext-in-nestjs-middleware)                                                                                                                                                                                                                                                                   |
| 42  | [How can you implement soft deletes in NestJS using TypeORM, and why might soft deletes be preferred over hard deletes?](#how-can-you-implement-soft-deletes-in-nestjs-using-typeorm-and-why-might-soft-deletes-be-preferred-over-hard-deletes)                                                                                                                                                          |
| 43  | [Explain the concept of environment variables in NestJS, and how can they be utilized for configuration management?](#explain-the-concept-of-environment-variables-in-nestjs-and-how-can-they-be-utilized-for-configuration-management)                                                                                                                                                                  |
| 44  | [What is the role of migration scripts in TypeORM, and how can you create and run migrations in a NestJS application?](#what-is-the-role-of-migration-scripts-in-typeorm-and-how-can-you-create-and-run-migrations-in-a-nestjs-application)                                                                                                                                                              |
| 45  | [What is the purpose of ExecutionContext in NestJS?](#what-is-the-purpose-of-executioncontext-in-nestjs)                                                                                                                                                                                                                                                                                                 |
| 46  | [What is the purpose of the @Res() decorator in NestJS controllers?](#what-is-the-purpose-of-the-res-decorator-in-nestjs-controllers)                                                                                                                                                                                                                                                                    |
| 47  | [Explain the various Modules in NestJS?](#explain-the-various-modules-in-nestjs)                                                                                                                                                                                                                                                                                                                         |
| 48  | [How can you secure your NestJS application?](#how-can-you-secure-your-nestjs-application)                                                                                                                                                                                                                                                                                                               |
| 49  | [What is the entry file of NestJs application?](#what-is-the-entry-file-of-nestjs-application)                                                                                                                                                                                                                                                                                                           |
| 50  | [What is the difference between dependency injection and inversion of control (IoC)?](#what-is-the-difference-between-dependency-injection-and-inversion-of-control-ioc)                                                                                                                                                                                                                                 |
| 51  | [How can you implement Caching in NestJS?](#how-can-you-implement-caching-in-nestjs)                                                                                                                                                                                                                                                                                                                     |
| 52  | [Explain the purpose of the Dependency Inversion Principle (DIP) in NestJS?](#explain-the-purpose-of-the-dependency-inversion-principle-dip-in-nestjs)                                                                                                                                                                                                                                                   |
| 53  | [How can you schedule tasks in NestJS?](#how-can-you-schedule-tasks-in-nestjs)                                                                                                                                                                                                                                                                                                                           |
| 54  | [How can you handle database transactions in NestJS, and why are transactions important in certain scenarios?](#how-can-you-handle-database-transactions-in-nestjs-and-why-are-transactions-important-in-certain-scenarios)                                                                                                                                                                              |
| 55  | [How can you implement versioning in NestJS APIs?](#how-can-you-implement-versioning-in-nestjs-api)                                                                                                                                                                                                                                                                                                      |
| 56  | [Explain the purpose of the `@nestjs/graphql Resolver` and `@nestjs/graphql Scalar` decorators, and how they relate to GraphQL in NestJS?](#explain-the-purpose-of-the-nestjs-graphql-resolver-and-nestjs-graphql-scalar-decorators-and-how-they-relate-to-graphql-in-nestjs)                                                                                                                            |
| 57  | [Explain the concept of Serialization and Deserialization in NestJS?](#explain-the-concept-of-serialization-and-deserialization-in-nestjs)                                                                                                                                                                                                                                                               |
| 58  | [Explain the role of NestJS middleware in the context of Microservices and provide a scenario where middleware is beneficial in a Microservices setup?](#explain-the-role-of-nestjs-middleware-in-the-context-of-microservices-and-provide-a-scenario-where-middleware-is-beneficial-in-a-microservices-setup)                                                                                           |
| 59  | [Discuss the different types of coupling, such as tight coupling and loose coupling, and provide examples of how NestJS modules contribute to achieving loose coupling in a modularized application?](#discuss-the-different-types-of-coupling-such-as-tight-coupling-and-loose-coupling-and-provide-examples-of-how-nestjs-modules-contribute-to-achieving-loose-coupling-in-a-modularized-application) |
| 60  | [How does NestJS support Server-Sent Events (SSE), and what are the primary advantages of using SSE for real-time communication in web applications?](#how-does-nestjs-support-server-sent-events-sse-and-what-are-the-primary-advantages-of-using-sse-for-real-time-communication-in-web-applications)                                                                                                  |

### Answers

  ### 1. What is NestJS?

    **NestJS is a Node.js framework used to build backend and server-side applications.** It helps developers create APIs and business logic in a clean, structured, and scalable way.

    NestJS is built with **TypeScript** and runs on the **Node.js** runtime. It gives the application a proper architecture so the code is not just thrown into one large file. Instead, developers organize the project into **modules**, **controllers**, **services**, **providers**, **middlewares**, and **guards**.

    This modular approach makes backend development easier to maintain and scale. For example, a project can have separate areas for:

    - Users
    - Products
    - Orders
    - Payments
    - Authentication

    Each part can have its own controller and service, which improves code organization and team collaboration.

    NestJS also supports many modern backend features, including:

    - REST APIs
    - Validation
    - Authentication and authorization
    - Database integration
    - WebSockets
    - Microservices
    - GraphQL
    - Dependency Injection

    A simple flow in NestJS looks like this:

    ```text
    Client -> Controller -> Service -> Database -> Response
    ```

    In simple words, **NestJS is a structured backend framework for Node.js that helps us build clean, scalable, and maintainable applications using TypeScript.**

    **Interview answer:** NestJS is a TypeScript-based Node.js backend framework used to build scalable, maintainable server-side applications and APIs. It provides a modular architecture with controllers, services, modules, and dependency injection, which helps developers write organized and testable code. It is widely used for building enterprise-grade backend systems and supports features such as authentication, validation, databases, microservices, and GraphQL.

    **[⬆ Back to Top](#table-of-contents)**

2.  ### 2. Who developed NestJS? Why did they develop NestJS?

    **NestJS was developed by Kamil Myśliwiec.** He created it to solve a common problem in the Node.js ecosystem: many backend applications were becoming unstructured, difficult to maintain, and hard to scale.

    He wanted to bring the clean architecture and maintainability ideas from frameworks like **Angular** into the backend world. NestJS uses a modular structure and dependency injection, which makes backend code more predictable and easier to manage as applications grow.

    In other words, NestJS was designed to provide a professional architecture for building large server-side applications without losing the flexibility of JavaScript and TypeScript.

    It became popular because it combines the best ideas from Angular, Express, and modern backend patterns, making it a great option for enterprise applications, APIs, and microservices.

    **[⬆ Back to Top](#table-of-contents)**

3.  ### 3. When was NestJS first released?

    **NestJS was first released in 2017.** It was introduced as a framework that brought a structured and modular approach to backend development in the Node.js ecosystem.

    Since its release, it has gained strong popularity among developers because of its TypeScript-first approach, dependency injection system, and clean architecture. Over time, it evolved into a robust framework used by many startups and large companies for building APIs, web apps, and microservices.

    **[⬆ Back to Top](#table-of-contents)**

4.  ### 4. How can you install NestJS and set up a new project on your machine?

    To work with NestJS, you first need **Node.js** and **npm** installed on your machine. After that, you can install the NestJS CLI globally using the following command:

    ```bash
    npm install -g @nestjs/cli
    ```

    Once installed, you can create a new project with:

    ```bash
    nest new project-name
    ```

    This command creates a basic NestJS application with the required folder structure. After that, you can run the app with:

    ```bash
    cd project-name
    npm run start
    ```

    NestJS also provides generators to create modules, controllers, services, and resources very quickly. For example:

    ```bash
    nest generate module users
    ```

    or

    ```bash
    nest g resource users
    ```

    This helps generate the common files needed for CRUD operations, such as:

    - users.controller.ts
    - users.service.ts
    - users.module.ts
    - DTO files for validation

    The CLI saves time and helps developers follow the NestJS architecture from the beginning.

    **[⬆ Back to Top](#table-of-contents)**

5.  ### 5. What’s the difference between NestJS and Angular?

    **Angular** and **NestJS** are both inspired by the same architectural thinking, but they are used for different parts of the application.

    **Angular** is a frontend framework used to build client-side applications and user interfaces. It is mainly used for web applications that run in the browser.

    **NestJS** is a backend framework used to build server-side logic, APIs, and business systems. It runs on Node.js and is focused on backend architecture.

    Both frameworks share concepts like:

    - Modules
    - Dependency injection
    - Decorators
    - Service-based design

    However, Angular is mainly for the UI layer, while NestJS is mainly for the server layer. In other words, Angular helps build the front-end experience, and NestJS helps build the backend logic that supports that experience.

    **[⬆ Back to Top](#table-of-contents)**

6.  ### 6. Is it possible to use other languages like C++, Ruby, or Python with NestJS? If yes, then how?

    **NestJS is built on Node.js, so it primarily uses JavaScript or TypeScript.** It is not designed to directly run languages like Python, Ruby, or C++ inside the same application runtime. However, that does not mean you cannot use those languages in a larger system.

    In real-world applications, a NestJS project can communicate with other services built in different languages using:

    - HTTP APIs
    - gRPC
    - Message queues
    - RabbitMQ
    - Kafka
    - WebSockets

    For example, you may build a Python service for machine learning and expose it through an API. Then your NestJS application can call that Python service as a client. This is a common pattern in microservices architecture.

    So, NestJS itself is not a cross-language runtime, but it can easily work alongside services written in other languages when those services communicate through standard protocols.

    **[⬆ Back to Top](#table-of-contents)**

7.  ### 7. What are the main components of a NestJS application?

    A NestJS application is usually organized into a few core building blocks that make the project easier to maintain.

    **Modules**: Modules group related features together. For example, a UserModule may contain user-related controllers, services, and providers.

    **Controllers**: Controllers handle incoming HTTP requests and return responses to the client.

    **Services**: Services contain the business logic and are often used to interact with databases or other systems.

    **Providers**: Providers are the objects that NestJS manages through dependency injection. Services are often providers, but providers can also be values, factories, and other custom objects.

    **Middleware**: Middleware runs before the request reaches the route handler and is useful for logging, authentication, or request modification.

    **Guards**: Guards decide whether a request is allowed to continue based on rules such as authentication or role checks.

    **Pipes**: Pipes validate and transform data before it reaches the controller logic.

    **Interceptors**: Interceptors can modify incoming requests or outgoing responses and are often used for logging, transformation, or metrics.

    These components together give NestJS a structured architecture that separates responsibilities cleanly.

    **[⬆ Back to Top](#table-of-contents)**

8.  ### 8. How to declare a class as a controller in NestJS?

    In NestJS, we declare a class as a controller by using the **@Controller()** decorator. This tells NestJS that the class should handle incoming requests from a given route.

    Example:

    ```typescript
    import { Controller, Get } from '@nestjs/common';

    @Controller('example')
    export class ExampleController {
      @Get()
      getHello(): string {
        return 'Hello World!';
      }
    }
    ```

    Here, `@Controller('example')` means this controller will handle requests related to the `/example` route. The `@Get()` decorator tells NestJS that the method should respond to an HTTP GET request.

    Controllers are responsible for receiving the request, calling the appropriate service or logic, and sending back a response.

    **[⬆ Back to Top](#table-of-contents)**

9.  ### 9. Can you explain how to use decorators in a NestJS controller?

    Decorators are one of the most important parts of NestJS. They are special functions with the `@` symbol and are used to attach metadata to classes, methods, and parameters.

    In NestJS, decorators help define the behavior of controllers and routes. Some common decorators are:

    - `@Controller()` — marks a class as a controller
    - `@Get()` — handles GET requests
    - `@Post()` — handles POST requests
    - `@Put()` — handles PUT requests
    - `@Delete()` — handles DELETE requests
    - `@Param()` — reads route parameters
    - `@Body()` — reads request body

    Example:

    ```typescript
    import {
      Controller,
      Get,
      Post,
      Put,
      Delete,
      Param,
      Body,
    } from '@nestjs/common';

    @Controller('cats')
    export class CatsController {
      @Get()
      findAll(): string {
        return 'Return all cats';
      }

      @Get(':id')
      findOne(@Param('id') id: number): string {
        return `Return cat with id ${id}`;
      }

      @Post()
      create(@Body() body: any): string {
        return `Create cat with body ${JSON.stringify(body)}`;
      }

      @Put(':id')
      update(@Param('id') id: number, @Body() body: any): string {
        return `Update cat ${id}`;
      }

      @Delete(':id')
      remove(@Param('id') id: number): string {
        return `Delete cat ${id}`;
      }
    }
    ```

    This shows how decorators make route definitions and request handling very easy and readable.

    **[⬆ Back to Top](#table-of-contents)**

10. ### 10. How can you use route parameters in a NestJS controller?

    Route parameters are values passed as part of the URL. In NestJS, we can access them using the `@Param()` decorator.

    Example:

    ```typescript
    @Get(':id')
    getUser(@Param('id') id: string) {
      return `User ID is ${id}`;
    }
    ```

    If the client sends a request like `/users/42`, then the value `42` is captured in the `id` parameter and passed into the method.

    This is very useful when we need to fetch a specific record from the database, such as a user, product, or order by ID.

    **[⬆ Back to Top](#table-of-contents)**

11. ### 11. What is the role of the `@Body()` decorator?

    The `@Body()` decorator is used to extract the data sent in the request body of an HTTP request. In NestJS, this is especially useful when the client sends JSON data to create or update a resource.

    For example, when a frontend sends a POST request to register a new user, the data is usually included in the request body. The server can read that data using `@Body()` and pass it directly to the controller method.

    Example:

    ```typescript
    @Post('users')
    createUser(@Body() userDto: CreateUserDto) {
      return this.usersService.create(userDto);
    }
    ```

    In this example, the incoming JSON body is automatically converted into an object matching the DTO shape and passed to the `createUser` method. This makes request handling cleaner and helps with validation.

    Without `@Body()`, the controller would have no direct access to the incoming payload. So this decorator is essential for processing form data, JSON requests, and API payloads.

    **[⬆ Back to Top](#table-of-contents)**

12. ### 12. What is an interceptor in the context of NestJS?

    An **interceptor** in NestJS is a class that can intercept the request before it reaches the route handler and also intercept the response before it is sent back to the client. It is commonly used for cross-cutting concerns such as logging, response transformation, caching, authentication, and error handling.

    Interceptors are decorated with `@Injectable()` and implement the `NestInterceptor` interface. They work in a way similar to aspect-oriented programming, where a common action can be applied around a method execution without modifying the business logic itself.

    Example:

    ```typescript
    import {
      Injectable,
      NestInterceptor,
      ExecutionContext,
      CallHandler,
    } from '@nestjs/common';
    import { Observable } from 'rxjs';
    import { tap } from 'rxjs/operators';

    @Injectable()
    export class LoggingInterceptor implements NestInterceptor {
      intercept(context: ExecutionContext, next: CallHandler): Observable<any> {
        console.log('Before request');
        const now = Date.now();

        return next.handle().pipe(
          tap(() => console.log(`After request: ${Date.now() - now}ms`)),
        );
      }
    }
    ```

    In this example, the interceptor logs before and after the request is processed. It does not change the business logic, but it adds useful monitoring and execution timing information.

    **[⬆ Back to Top](#table-of-contents)**

13. ### 13. What are pipes in the context of NestJS?

    A **pipe** in NestJS is a class used to validate or transform input data before it is passed to the controller or service. Pipes are very useful when you want to ensure the request payload follows the expected rules.

    Every pipe implements the `PipeTransform` interface and is usually decorated with `@Injectable()`. It can either:

    - transform the value,
    - validate the value,
    - or throw an exception if the value is invalid.

    Example:

    ```typescript
    import {
      PipeTransform,
      Injectable,
      BadRequestException,
    } from '@nestjs/common';

    @Injectable()
    export class ParseIntPipe implements PipeTransform<string, number> {
      transform(value: string): number {
        const parsed = Number(value);
        if (Number.isNaN(parsed)) {
          throw new BadRequestException('Invalid number');
        }
        return parsed;
      }
    }
    ```

    This pipe converts a string parameter into a number, and throws an error if the input is not valid.

    Common built-in pipes include `ValidationPipe`, `ParseIntPipe`, `ParseUUIDPipe`, `ParseBoolPipe`, and `DefaultValuePipe`. They help developers keep validation logic organized and reusable.

    **[⬆ Back to Top](#table-of-contents)**

14. ### 14. What are guards in the context of NestJS?

    A **guard** is a class responsible for deciding whether a request should proceed to the route handler or be rejected. Guards are mainly used for access control, such as authentication and authorization.

    In NestJS, a guard implements the `CanActivate` interface and returns either `true` or `false` (or a Promise/Observable resolving to a boolean).

    Example:

    ```typescript
    import { Injectable, CanActivate, ExecutionContext } from '@nestjs/common';

    @Injectable()
    export class AuthGuard implements CanActivate {
      canActivate(context: ExecutionContext): boolean {
        const request = context.switchToHttp().getRequest();
        return !!request.user;
      }
    }
    ```

    If `request.user` exists, the request continues; otherwise it is blocked. This is commonly used to protect routes that require login or specific roles.

    Guards are a clean way to separate security checks from business logic, which makes the application easier to manage and secure.

    **[⬆ Back to Top](#table-of-contents)**

15. ### 15. What are middlewares in the context of NestJS?

    Middleware in NestJS works similarly to Express middleware. It runs before the request reaches the route handler and can inspect or modify the request and response objects.

    Middleware is often used for:

    - logging requests,
    - checking headers,
    - request validation,
    - authentication checks,
    - rewriting or modifying requests.

    Middleware receives the `req`, `res`, and `next` objects, and if it does not end the request itself, it must call `next()` to continue the chain.

    Example:

    ```typescript
    import { Injectable, NestMiddleware } from '@nestjs/common';

    @Injectable()
    export class LoggerMiddleware implements NestMiddleware {
      use(req: any, res: any, next: () => void) {
        console.log('Request received:', req.method, req.url);
        next();
      }
    }
    ```

    Middleware is useful for generic, request-level logic that should apply to many routes without adding repeated code inside each controller.

    **[⬆ Back to Top](#table-of-contents)**

16. ### 16. Explain the concept of Dependency Injection in NestJS. How does it help in building modular and testable applications?

    **Dependency Injection (DI)** is a design pattern where an object receives its dependencies from outside instead of constructing them inside itself. This is one of the core principles of NestJS.

    In NestJS, the framework creates and manages objects automatically based on the metadata and the type information. This is called the **Inversion of Control (IoC)** container.

    Example:

    ```typescript
    @Injectable()
    export class UserService {
      getUsers(): string[] {
        return ['Alice', 'Bob'];
      }
    }

    @Controller('users')
    export class UserController {
      constructor(private readonly userService: UserService) {}

      @Get()
      getUsers() {
        return this.userService.getUsers();
      }
    }
    ```

    Here, `UserController` does not create `UserService` manually. NestJS injects it automatically. This makes the application more modular, easier to test, and easier to maintain.

    The benefits of DI include:

    - Reusability of components
    - Easy mocking in unit tests
    - Better separation of concerns
    - Cleaner architecture

    In practical terms, DI allows different parts of the project to depend on abstractions rather than specific implementations, which is especially helpful in large applications.

    **[⬆ Back to Top](#table-of-contents)**

17. ### 17. What’s the difference between `@Injectable()` and `@Inject()` decorators?

    Both decorators are related to dependency injection, but they are used in different situations.

    **`@Injectable()`** marks a class as a provider that NestJS can create and inject. It is typically used on services or other classes that need to be available in the container.

    Example:

    ```typescript
    @Injectable()
    export class UserService {}
    ```

    **`@Inject()`** is used when we want to explicitly tell NestJS which dependency to inject, usually for non-class tokens, custom providers, or values.

    Example:

    ```typescript
    constructor(@Inject('CACHE_SERVICE') private readonly cacheService: any) {}
    ```

    In simple terms, `@Injectable()` is used to declare a class as a provider, while `@Inject()` is used to bind a specific dependency token to a constructor parameter.

    **[⬆ Back to Top](#table-of-contents)**

18. ### 18. How does the Nest logger differ from the standard `console.log()` and when would you prefer one over the other?

    The standard `console.log()` is fine for quick debugging during development, but it is not as structured as the NestJS logger. The NestJS logger provides built-in features like log levels, context, timestamps, and formatting.

    NestJS supports log levels such as:

    - `log`
    - `warn`
    - `debug`
    - `error`
    - `verbose`
    - `fatal`

    Example:

    ```typescript
    import { Logger } from '@nestjs/common';

    const logger = new Logger('AppService');
    logger.log('Application started successfully');
    logger.error('Something went wrong');
    ```

    This is useful in production systems because logs are easier to filter, analyze, and understand. In small scripts or rapid debugging, `console.log()` is simpler and faster, but for real applications, the Nest logger is more professional and reliable.

    **[⬆ Back to Top](#table-of-contents)**

19. ### 19. What is the difference between interceptors and middleware?

    Both interceptors and middleware can add logic before or after request handling, but they are used for different purposes.

    **Middleware** is request-level logic that sits in the HTTP pipeline. It is especially useful for tasks like logging, parsing headers, or checking cookies. It works mostly with HTTP requests and is similar to Express middleware.

    **Interceptors** are more advanced. They can also run before and after a method, but they can work with HTTP, WebSockets, and microservices. They can modify the response, transform output, and add additional behavior around method execution.

    So, if the requirement is to process the request itself before it reaches the controller, middleware is often appropriate. If the requirement is to change response behavior or apply cross-cutting logic around methods and services, an interceptor is a better fit.

    **[⬆ Back to Top](#table-of-contents)**

20. ### 20. What testing frameworks work best with NestJS?

    NestJS is compatible with several JavaScript and TypeScript testing tools, and the most commonly used framework is **Jest**. It is widely preferred because it is simple, fast, and easy to integrate with TypeScript projects.

    Other frameworks like **Mocha** and **Jasmine** can also be used, but Jest is usually the standard choice in NestJS projects because of its excellent support for mocking, assertions, and async testing.

    NestJS also provides a testing module through `@nestjs/testing`, which helps developers create test modules, inject mock dependencies, and test controllers and services in isolation.

    Example:

    ```typescript
    const moduleRef = await Test.createTestingModule({
      providers: [UserService],
    }).compile();
    ```

    Testing is important in NestJS because it helps verify that controllers, services, and guards behave correctly before deployment.

    **[⬆ Back to Top](#table-of-contents)**

21. ### 21. Explain the purpose of DTOs (Data Transfer Objects) in NestJS.

    A **DTO** is a class used to describe the shape of the data that is expected to be sent or received by an API. In NestJS, DTOs are commonly used with validation and request payloads so that each incoming request is checked before it reaches your business logic.

    DTOs are useful because they make the API contract clear. They define what fields are required, optional, and what type each field should have. For example, when creating a user, the API may expect a DTO with a `name`, `email`, and `password` field.

    Example:

    ```typescript
    import { IsString, IsEmail, MinLength } from 'class-validator';

    export class CreateUserDto {
      @IsString()
      name: string;

      @IsEmail()
      email: string;

      @IsString()
      @MinLength(6)
      password: string;
    }
    ```

    This DTO clearly defines the expected data and can be used with `ValidationPipe` to reject invalid input before the request reaches the service layer.

    DTOs also help in code readability, maintainability, and API documentation. They make complex APIs easier to understand and reduce errors caused by inconsistent data types.

    **[⬆ Back to Top](#table-of-contents)**

22. ### 22. How can you handle asynchronous operations in NestJS, and what is the role of the Promise object?

    Asynchronous operations are very common in backend applications because database queries, HTTP requests, file processing, and other operations may take time. NestJS supports asynchronous code using `async` and `await`, which allow the application to continue working without blocking the whole server.

    Example:

    ```typescript
    @Injectable()
    export class UserService {
      async getUserById(id: number): Promise<string> {
        const user = await this.fetchUserFromDb(id);
        return user;
      }
    }
    ```

    The `Promise` object represents a value that may be available now, later, or never. When a function returns a Promise, the caller can wait for it using `await`, and only continue once the task finishes.

    This is especially useful for database calls or API integration. When a request needs to fetch data from multiple sources, asynchronous handling ensures the server remains responsive and efficient.

    If the application needs to work with streams of values over time, NestJS also supports `Observable` from RxJS, but `Promise` is the standard choice for single asynchronous tasks.

    **[⬆ Back to Top](#table-of-contents)**

23. ### 23. Explain the purpose of the `@InjectRepository()` decorator in NestJS.

    The `@InjectRepository()` decorator is used when working with **TypeORM** to inject a repository into a service. A repository is a class that exposes methods to create, read, update, and delete records for a specific entity.

    Example:

    ```typescript
    import { Injectable } from '@nestjs/common';
    import { InjectRepository } from '@nestjs/typeorm';
    import { Repository } from 'typeorm';
    import { User } from './user.entity';

    @Injectable()
    export class UserService {
      constructor(
        @InjectRepository(User)
        private readonly userRepository: Repository<User>,
      ) {}

      findAll() {
        return this.userRepository.find();
      }
    }
    ```

    In this example, the `User` repository is injected into `UserService`, and then its methods are used to work with the database. This keeps the service clean and allows the database logic to be handled in a consistent, structured way.

    Without `@InjectRepository()`, the service would not easily have access to the database entity repository.

    **[⬆ Back to Top](#table-of-contents)**

24. ### 24. Explain the purpose of the `@nestjs/jwt` package in NestJS?

    The `@nestjs/jwt` package is used for working with **JSON Web Tokens (JWTs)** in NestJS. JWTs are commonly used for authentication and authorization because they allow the server to verify the identity of a user without needing to store session data on the server.

    This package helps with:

    - generating JWTs,
    - verifying incoming tokens,
    - decoding tokens,
    - protecting routes with guards.

    A common flow is:

    1. User logs in with correct credentials.
    2. Server creates a JWT containing user information.
    3. Client sends that token in the request header.
    4. NestJS validates the token and allows or denies access to protected routes.

    `@nestjs/jwt` is often used together with `Passport` and `AuthGuard` to implement secure login systems for APIs.

    **[⬆ Back to Top](#table-of-contents)**

25. ### 25. Discuss how tokens are used for authorization in an API. What is the difference between authentication and authorization, and how are these processes implemented with tokens?

    **Authentication** means verifying who the user is. For example, the user provides a username and password, and the server checks whether those credentials are valid.

    **Authorization** means verifying what that user is allowed to do. Once the user is authenticated, the server checks whether the user has permission to access a route, resource, or action.

    In JWT-based APIs, the server usually creates a token after successful login. The token is then attached to later requests in the `Authorization` header. The server validates the token and extracts user information from it.

    Example flow:

    1. User logs in.
    2. Server verifies credentials.
    3. Server creates JWT.
    4. Client sends JWT in subsequent requests.
    5. Server decodes and validates the token.
    6. Server checks permissions and allows or blocks the request.

    In simple words, authentication answers “Who are you?”, while authorization answers “Are you allowed to do this?”

    **[⬆ Back to Top](#table-of-contents)**

26. ### 26. Why is it important for tokens to have an expiration time? How can you implement token expiration in NestJS, and what role do refresh tokens play in maintaining user sessions?

    Tokens need an expiration time because if a token is stolen or leaked, it should not remain valid forever. Expiration reduces the risk of misuse and keeps the authentication system safer.

    In NestJS, when generating a JWT, you can set an expiration period such as 15 minutes or 1 hour:

    ```typescript
    this.jwtService.sign(payload, { expiresIn: '60s' });
    ```

    This means the token is valid only for 60 seconds from the time it is issued.

    However, short-lived access tokens can interrupt the user experience. That is where **refresh tokens** come in. A refresh token is a long-lived token used to obtain a new access token when the original one expires. This lets the user stay logged in without constantly re-entering credentials.

    A common strategy is to issue:

    - a short-lived access token for API access,
    - a longer-lived refresh token for reissuing the access token.

    **[⬆ Back to Top](#table-of-contents)**

27. ### 27. Describe the mechanism for a token refresh in NestJS. How can you implement an automatic token refresh strategy to maintain user sessions?

    A token refresh flow usually works like this:

    1. User logs in and receives both an access token and a refresh token.
    2. The access token is short-lived and used for normal API requests.
    3. When the access token expires, the client sends the refresh token to a dedicated endpoint.
    4. The server validates the refresh token.
    5. If valid, the server issues a new access token and optionally a new refresh token.

    This approach keeps the user session alive without forcing a full re-login. It is useful for applications like dashboards, mobile apps, and SaaS products where users expect a smooth experience.

    In practice, the refresh token is usually stored securely, often in a database or secure cookie, and should be invalidated on logout or suspicious activity. This helps prevent unauthorized reuse.

    **[⬆ Back to Top](#table-of-contents)**

28. ### 28. How does NestJS support authentication and authorization?

    NestJS supports authentication and authorization through a combination of built-in features and integration libraries.

    Some of the main mechanisms are:

    - **Passport.js** integration for common authentication strategies such as JWT, local login, OAuth, and more.
    - **`@nestjs/jwt`** for generating and validating JWTs.
    - **Guards** for deciding whether a request can access a route.
    - **Roles and decorators** for authorization checks.

    Example:

    ```typescript
    import { Controller, Post, Request, UseGuards } from '@nestjs/common';
    import { AuthGuard } from '@nestjs/passport';

    @Controller('auth')
    export class AuthController {
      @UseGuards(AuthGuard('local'))
      @Post('login')
      login(@Request() req) {
        return req.user;
      }
    }
    ```

    In this approach, guard logic handles authentication, and route-level authorization rules decide whether the user can access the endpoint.

    **[⬆ Back to Top](#table-of-contents)**

29. ### 29. What is the difference between Provider and Services in NestJS? Can we have a provider without an injectable decorator? Give examples.

    In NestJS, a **service** is a specific type of **provider**. All services are providers, but not all providers are services.

    A service usually contains business logic and is marked with `@Injectable()`:

    ```typescript
    @Injectable()
    export class UserService {
      getUsers() {
        return ['A', 'B', 'C'];
      }
    }
    ```

    A provider can also be something else, such as a value or a factory. For example:

    ```typescript
    const appProviders = [{
      provide: 'API_URL',
      useValue: 'https://example.com',
    }];
    ```

    Here, `API_URL` is a provider even though it is not a class or service. It is a string value that can be injected anywhere in the app.

    So yes, a provider does not always need `@Injectable()`. The decorator is mainly required when the provider is a class that depends on NestJS injection.

    **[⬆ Back to Top](#table-of-contents)**

30. ### 30. What are custom providers and how do they differ from standard providers in NestJS?

    A **standard provider** is usually a class decorated with `@Injectable()`. It can be created and injected by NestJS automatically.

    Example:

    ```typescript
    @Injectable()
    export class OrderService {}
    ```

    A **custom provider** is a provider that does not necessarily follow the default class-based pattern. It may provide a value, a factory, or an async object creation strategy.

    Example:

    ```typescript
    {
      provide: 'CONFIG',
      useValue: {
        port: 3000,
        env: 'development',
      },
    }
    ```

    Or a factory provider:

    ```typescript
    {
      provide: 'DB_CONNECTION',
      useFactory: () => createConnection(),
    }
    ```

    Custom providers give developers more flexibility when they need to register dynamic values, configuration objects, or custom initialization logic.

    **[⬆ Back to Top](#table-of-contents)**

31. ### 31. How can you generate API documentation using Swagger in NestJS? Discuss the importance of documenting your API and how it benefits developers.

    Swagger is a widely used tool for API documentation. In NestJS, it can be integrated using the `@nestjs/swagger` package.

    Example setup:

    ```typescript
    import { NestFactory } from '@nestjs/core';
    import { SwaggerModule, DocumentBuilder } from '@nestjs/swagger';
    import { AppModule } from './app.module';

    async function bootstrap() {
      const app = await NestFactory.create(AppModule);

      const config = new DocumentBuilder()
        .setTitle('My API')
        .setDescription('API documentation')
        .setVersion('1.0')
        .build();

      const document = SwaggerModule.createDocument(app, config);
      SwaggerModule.setup('api', app, document);

      await app.listen(3000);
    }
    bootstrap();
    ```

    This creates a Swagger UI at `/api`, where developers can view routes, request body examples, response models, and parameter details directly in the browser.

    API documentation is important because it helps developers understand how to use the backend correctly. It reduces confusion, speeds up integration, makes testing easier, and improves collaboration among frontend, backend, and QA teams.

    **[⬆ Back to Top](#table-of-contents)**

32. ### 32. Explain the purpose of the `@nestjs/swagger` `@ApiProperty()` and `@ApiOperation()` decorators.

    Swagger decorators help NestJS generate meaningful API documentation for controllers and DTOs.

    `@ApiProperty()` is used inside DTO classes to describe individual fields. It tells Swagger what each property represents and may include details like type, example, description, and validation constraints.

    Example:

    ```typescript
    import { ApiProperty } from '@nestjs/swagger';

    export class CreateUserDto {
      @ApiProperty({ example: 'John Doe' })
      name: string;

      @ApiProperty({ example: 'john@example.com' })
      email: string;
    }
    ```

    `@ApiOperation()` is used on controller methods to describe the endpoint itself, such as its summary or purpose.

    Example:

    ```typescript
    @Post()
    @ApiOperation({ summary: 'Create a new user' })
    createUser(@Body() dto: CreateUserDto) {
      return dto;
    }
    ```

    These decorators make Swagger documentation clear, structured, and developer-friendly.

    **[⬆ Back to Top](#table-of-contents)**

33. ### 33. Explain the purpose of the Dockerfile in a NestJS application, and how it facilitates containerization.

    A **Dockerfile** is a file that defines how an application should be built into a Docker image. In a NestJS application, it helps package the project with its dependencies and runtime environment so it can run consistently anywhere.

    Example:

    ```dockerfile
    FROM node:18-alpine
    WORKDIR /app
    COPY package*.json ./
    RUN npm install
    COPY . .
    EXPOSE 3000
    CMD ["npm", "run", "start"]
    ```

    This allows the NestJS app to be containerized and run in a consistent environment. Docker ensures the code, Node.js version, dependencies, and system configuration are bundled together, reducing the classic problem of “it works on my machine.”

    Containerization makes deployment easier, improves portability, and supports modern CI/CD and cloud environments.

    **[⬆ Back to Top](#table-of-contents)**

34. ### 34. How can you use Docker Compose with NestJS, and what is its role in a multi-container setup?

    **Docker Compose** is used to define and run multiple containers together. In a NestJS app, this is especially useful when the application depends on a database, cache, or other service.

    Example `docker-compose.yml`:

    ```yaml
    version: '3'
    services:
      app:
        build: .
        ports:
          - '3000:3000'
        depends_on:
          - db

      db:
        image: postgres:15
        environment:
          POSTGRES_USER: postgres
          POSTGRES_PASSWORD: postgres
          POSTGRES_DB: appdb
    ```

    This file starts both the NestJS application and the PostgreSQL database together. Docker Compose keeps the startup process simple and ensures services start in the right order.

    In a multi-container architecture, Compose helps manage networking, startup dependencies, environment variables, and service orchestration from a single configuration file.

    **[⬆ Back to Top](#table-of-contents)**

35. ### 35. What is the purpose of the `@nestjs/passport` package, and how does it facilitate authentication in NestJS?

    The `@nestjs/passport` package integrates NestJS with the popular **Passport.js** authentication library. It allows developers to plug in different authentication strategies such as local login, JWT, OAuth, and social login.

    This package makes authentication easier to structure and test because it follows the same modular design as NestJS. Instead of writing custom auth logic everywhere, you can create a guard and a strategy and then reuse them across routes.

    Example:

    ```typescript
    @Injectable()
    export class JwtAuthGuard extends AuthGuard('jwt') {}
    ```

    This gives a clean and maintainable way to protect routes based on a valid token or login session.

    **[⬆ Back to Top](#table-of-contents)**

36. ### 36. How can you handle file uploads in NestJS, and what is the role of the Multer library?

    NestJS supports file uploads via the `@UseInterceptors()` decorator and the `FileInterceptor` or `FilesInterceptor` utilities. These interceptors allow uploaded files to be received from the request and processed by the controller.

    Example:

    ```typescript
    @Post('upload')
    @UseInterceptors(FileInterceptor('file'))
    uploadFile(@UploadedFile() file: Express.Multer.File) {
      return file.originalname;
    }
    ```

    The **Multer** library is the underlying middleware used for handling multipart form-data, which is how files are uploaded in HTTP requests. It parses the uploaded file and exposes the file metadata and buffer in the request.

    This makes file handling straightforward for features like profile images, documents, CSV uploads, and media files.

    **[⬆ Back to Top](#table-of-contents)**

37. ### 37. How does NestJS handle database interactions, and what are the supported databases?

    NestJS does not directly enforce a single database system. Instead, it provides a modular structure that allows developers to choose the database technology they want, such as TypeORM, Prisma, Mongoose, or Sequelize.

    Common database integrations in NestJS include:

    - **TypeORM** for PostgreSQL, MySQL, MariaDB, SQLite, SQL Server, and more.
    - **Mongoose** for MongoDB.
    - **Sequelize** for PostgreSQL, MySQL, SQLite, and SQL Server.
    - **Prisma** for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB, and other supported databases.

    These libraries integrate smoothly with NestJS modules and services, allowing the database layer to stay organized and easy to maintain.

    **[⬆ Back to Top](#table-of-contents)**

38. ### 38. What is a circular dependency (dependency cycle) in NestJS, and how can it be fixed?

    A **circular dependency** occurs when two classes or modules depend on each other directly or indirectly. For example, `ServiceA` depends on `ServiceB`, and `ServiceB` depends on `ServiceA`.

    This can create initialization problems because NestJS cannot always resolve the dependency graph cleanly.

    One common solution is `forwardRef()`, which allows a class to reference a provider that is still being defined.

    Example:

    ```typescript
    @Injectable()
    export class UserService {
      constructor(
        @Inject(forwardRef(() => ProfileService))
        private readonly profileService: ProfileService,
      ) {}
    }
    ```

    Another approach is to redesign the architecture so that dependencies flow in one direction. Circular dependencies often indicate that responsibilities are mixed together and should be separated into cleaner modules or interfaces.

    **[⬆ Back to Top](#table-of-contents)**

39. ### 39. How can you handle errors in NestJS?

    NestJS provides a structured way to handle errors using exceptions. Instead of returning raw errors, the framework allows you to throw HTTP-specific exceptions that are converted into proper responses.

    Example:

    ```typescript
    throw new NotFoundException('User not found');
    ```

    This results in an HTTP 404 error with a meaningful message. NestJS also includes other built-in exceptions such as:

    - `BadRequestException`
    - `UnauthorizedException`
    - `ForbiddenException`
    - `ConflictException`
    - `InternalServerErrorException`

    You can also create custom exception filters to handle errors globally and return a consistent response format across the whole application.

    **[⬆ Back to Top](#table-of-contents)**

40. ### 40. How does NestJS handle CORS (Cross-Origin Resource Sharing)?

    **CORS** allows a browser to allow requests from another origin, which is important when a frontend app runs on a different domain or port than the API server.

    In NestJS, CORS can be enabled globally in the bootstrap file:

    ```typescript
    const app = await NestFactory.create(AppModule);
    app.enableCors({
      origin: 'http://localhost:3000',
      methods: 'GET,HEAD,PUT,PATCH,POST,DELETE',
      credentials: true,
    });
    await app.listen(3000);
    ```

    This allows the frontend to access the backend securely while still restricting which origins are allowed. CORS configuration is important for security because it controls which clients can interact with the API.

    **[⬆ Back to Top](#table-of-contents)**

41. ### 41. Explain the purpose of the `ExecutionContext` in NestJS middleware.

    `ExecutionContext` gives access to the current request lifecycle and execution details. It is useful when you need to inspect the request, response, or route metadata while a request is being processed.

    In middleware and guards, it can help determine things like:

    - which route is being called,
    - what the incoming request looks like,
    - whether the request is HTTP, RPC, or WebSocket-based,
    - which arguments are being passed into the handler.

    This makes `ExecutionContext` a flexible object for building custom request-level logic without tightly coupling code to a specific route or framework implementation.

    **[⬆ Back to Top](#table-of-contents)**

42. ### 42. How can you implement soft deletes in NestJS using TypeORM, and why might soft deletes be preferred over hard deletes?

    A **soft delete** does not permanently remove data from the database. Instead, it marks the record as deleted while keeping it in the table.

    In TypeORM, this is commonly done with the `@DeleteDateColumn()` decorator:

    ```typescript
    import { Entity, PrimaryGeneratedColumn, Column, DeleteDateColumn } from 'typeorm';

    @Entity()
    export class User {
      @PrimaryGeneratedColumn()
      id: number;

      @Column()
      name: string;

      @DeleteDateColumn()
      deletedAt?: Date;
    }
    ```

    When a record is soft deleted, the `deletedAt` field is set instead of removing the row completely. This helps with data recovery, auditing, and maintaining referential integrity.

    Soft deletes are often preferred over hard deletes when the data may need to be restored later or when historical records must remain available for reporting or compliance.

    **[⬆ Back to Top](#table-of-contents)**

43. ### 43. Explain the concept of environment variables in NestJS, and how can they be utilized for configuration management?

    **Environment variables** are values stored outside the codebase, usually in a `.env` file or OS environment, and they are used to handle configuration that may change between environments such as development, testing, and production.

    Common examples include:

    - database URLs,
    - API keys,
    - port numbers,
    - JWT secrets.

    NestJS supports this via `@nestjs/config` and `ConfigModule`:

    ```typescript
    import { Module } from '@nestjs/common';
    import { ConfigModule } from '@nestjs/config';

    @Module({
      imports: [ConfigModule.forRoot()],
    })
    export class AppModule {}
    ```

    This allows configuration values to be read from `process.env` and managed centrally, which is safer and cleaner than hard-coding secrets into the source code.

    **[⬆ Back to Top](#table-of-contents)**

44. ### 44. What is the role of migration scripts in TypeORM, and how can you create and run migrations in a NestJS application?

    **Migrations** are used to manage database schema changes over time. They keep database structure changes versioned and predictable, especially in team environments and production deployments.

    In TypeORM, migrations help you:

    - add or remove tables,
    - modify columns,
    - create indexes,
    - update schema safely.

    You typically set the migration path in the TypeORM config and then generate or run them with the CLI:

    ```bash
    typeorm migration:generate -n AddUserTable
    typeorm migration:run
    ```

    These migrations are stored as versioned files and can be reverted when needed. This makes schema changes controlled, traceable, and easy to manage across environments.

    **[⬆ Back to Top](#table-of-contents)**

45. ### 45. What is the purpose of `ExecutionContext` in NestJS?

    `ExecutionContext` provides information about the current request and the method being executed. It is often used in guards, interceptors, and custom decorators to access details like the request object, route metadata, and execution context.

    It acts as an abstraction layer over the runtime environment so that the same logic can work across HTTP, WebSockets, and microservices scenarios.

    In simple terms, it tells NestJS “what is currently being executed, and in what context?”

    **[⬆ Back to Top](#table-of-contents)**

46. ### 46. What is the purpose of the `@Res()` decorator in NestJS controllers?

    The `@Res()` decorator gives direct access to the underlying HTTP response object. This is useful when you want to control the response manually, such as setting status codes, headers, or sending custom output.

    Example:

    ```typescript
    import { Controller, Get, Res } from '@nestjs/common';
    import { Response } from 'express';

    @Controller('cats')
    export class CatsController {
      @Get()
      findAll(@Res() res: Response) {
        res.status(200).send('This action returns all cats');
      }
    }
    ```

    This gives more flexibility than the default NestJS response handling, but it also puts more responsibility on the developer to send the response correctly.

    **[⬆ Back to Top](#table-of-contents)**

47. ### 47. Explain the various modules in NestJS.

    Modules are a core concept in NestJS. A module is a class decorated with `@Module()`, and it organizes the application into logical groups based on feature or responsibility.

    Common types of modules include:

    - **Feature modules**: groups related controllers and services.
    - **Shared modules**: provide reusable providers across multiple modules.
    - **Global modules**: available without needing to import them everywhere.
    - **Dynamic modules**: created with configuration to support different runtime setups.

    Example:

    ```typescript
    @Module({
      controllers: [UserController],
      providers: [UserService],
      exports: [UserService],
    })
    export class UserModule {}
    ```

    Modules help keep the application clean, modular, and easier to maintain as it grows.

    **[⬆ Back to Top](#table-of-contents)**

48. ### 48. How can you secure your NestJS application?

    Securing a NestJS application requires a combination of measures such as authentication, authorization, validation, rate limiting, and proper configuration.

    Some common approaches are:

    - using JWT-based auth with `@nestjs/jwt` and Passport,
    - protecting routes with Guards,
    - validating request input with `ValidationPipe`,
    - using HTTPS in production,
    - configuring CORS carefully,
    - adding rate limiting with `@nestjs/throttler`.

    Security is not a single step; it is a continuous process. Proper architecture, clean validation, and careful handling of credentials are essential for building reliable backend systems.

    **[⬆ Back to Top](#table-of-contents)**

49. ### 49. What is the entry file of a NestJS application?

    The main entry file of a NestJS project is usually `main.ts`. This file creates the NestJS application and starts the server.

    Example:

    ```typescript
    import { NestFactory } from '@nestjs/core';
    import { AppModule } from './app.module';

    async function bootstrap() {
      const app = await NestFactory.create(AppModule);
      await app.listen(3000);
    }
    bootstrap();
    ```

    The `bootstrap()` function initializes the root application module and starts listening for incoming requests on the chosen port.

    **[⬆ Back to Top](#table-of-contents)**

50. ### 50. What is the difference between dependency injection and inversion of control (IoC)?

    **Inversion of Control (IoC)** is a broad design principle where control of object creation and flow is moved out of the class itself and into a framework or container.

    **Dependency Injection (DI)** is one implementation of IoC. In NestJS, dependencies are injected into classes through constructors, so the class does not need to manually create them.

    This means the framework is controlling object wiring, while the application code focuses on business logic. The result is cleaner architecture, easier testing, and better modularity.

    **[⬆ Back to Top](#table-of-contents)**

51. ### 51. How can you implement caching in NestJS?

    Caching is used to reduce repeated work and improve performance by storing frequently used data temporarily. In NestJS, the `@nestjs/cache-manager` package is commonly used for this purpose.

    Example:

    ```typescript
    import { Module } from '@nestjs/common';
    import { CacheModule } from '@nestjs/cache-manager';

    @Module({
      imports: [CacheModule.register()],
    })
    export class AppModule {}
    ```

    After that, you can use the cache manager to store and retrieve values quickly. Caching is especially useful for API responses, database lookups, and repeated expensive computations.

    **[⬆ Back to Top](#table-of-contents)**

52. ### 52. Explain the purpose of the Dependency Inversion Principle (DIP) in NestJS.

    The **Dependency Inversion Principle** is one of the SOLID principles. It says that high-level modules should not depend on low-level modules; both should depend on abstractions.

    In NestJS, this is reflected in the use of interfaces, abstraction, and dependency injection. Instead of a service depending tightly on a concrete class, it depends on an abstraction or contract. This makes the application more flexible and easier to replace or test.

    For example, a service can depend on a repository interface, and different implementations can be swapped without changing the service logic. This reduces coupling and improves maintainability.

    **[⬆ Back to Top](#table-of-contents)**

53. ### 53. How can you schedule tasks in NestJS?

    NestJS supports scheduled tasks using the `@nestjs/schedule` package, which is built on top of the cron library.

    Example:

    ```typescript
    import { Injectable } from '@nestjs/common';
    import { Cron, CronExpression } from '@nestjs/schedule';

    @Injectable()
    export class TasksService {
      @Cron(CronExpression.EVERY_5_SECONDS)
      handleCron() {
        console.log('Running every 5 seconds');
      }
    }
    ```

    This is useful for periodic cleanup tasks, report generation, email reminders, syncing data, or health checks.

    **[⬆ Back to Top](#table-of-contents)**

54. ### 54. How can you handle database transactions in NestJS, and why are transactions important in certain scenarios?

    A **transaction** ensures that a set of database operations succeeds or fails together. This is important when multiple changes must be treated as one atomic unit.

    In NestJS, transactions are commonly handled with TypeORM or other ORMs. If one operation fails, the transaction can be rolled back so the database remains consistent.

    This is especially important in financial systems, order processing, user registration with related records, and payment flows. Without transactions, partial updates may leave the system in an invalid state.

    **[⬆ Back to Top](#table-of-contents)**

55. ### 55. How can you implement versioning in NestJS APIs?

    API versioning allows you to maintain multiple versions of the same endpoint while keeping the application backward compatible.

    NestJS supports multiple strategies such as:

    - URI versioning,
    - header versioning,
    - media type versioning,
    - custom versioning.

    Example:

    ```typescript
    app.enableVersioning({
      type: VersioningType.URI,
    });
    ```

    This makes it easier to evolve the API without breaking existing clients and is particularly useful in long-lived production applications.

    **[⬆ Back to Top](#table-of-contents)**

56. ### 56. Explain the purpose of the `@nestjs/graphql` `@Resolver()` and `@Scalar()` decorators, and how they relate to GraphQL in NestJS.

    GraphQL is a query language for APIs that allows clients to request exactly the data they need. NestJS integrates with GraphQL through the `@nestjs/graphql` package.

    `@Resolver()` marks a class as a GraphQL resolver. Resolvers contain the logic for fetching and returning data for the schema.

    `@Scalar()` is used for custom scalar types such as `Date`, `JSON`, or other special field types that are not already covered by GraphQL’s built-in scalar types.

    Together, they help developers build a GraphQL API in a structured way while keeping the schema and logic aligned with TypeScript classes.

    **[⬆ Back to Top](#table-of-contents)**

57. ### 57. Explain the concept of serialization and deserialization in NestJS.

    **Serialization** is the process of converting an object into a format that can be transmitted or stored, usually JSON.

    **Deserialization** is the reverse process—turning JSON or another format back into an object that an application can use.

    In NestJS, this is important when data moves between the database, service layer, controllers, and HTTP clients. For example, an entity may be transformed into a clean response object before it is returned to the client.

    Tools like DTOs and class-transformer help control this process and avoid exposing sensitive fields unnecessarily.

    **[⬆ Back to Top](#table-of-contents)**

58. ### 58. Explain the role of NestJS middleware in the context of microservices and provide a scenario where middleware is beneficial.

    Middleware in NestJS can be used to handle cross-cutting concerns before a request reaches a handler. In a microservices architecture, this is useful for tasks such as authentication, logging, tracing, request enrichment, and validation.

    Example scenario:

    A gateway service receives many internal requests from different services. Middleware can log request metadata, validate headers, and attach a correlation ID to every request before it is forwarded to the downstream microservice.

    This makes debugging easier, improves observability, and keeps each microservice from repeating the same cross-cutting logic.

    **[⬆ Back to Top](#table-of-contents)**

59. ### 59. Discuss the different types of coupling, such as tight coupling and loose coupling, and provide examples of how NestJS modules contribute to achieving loose coupling in a modularized application.

    **Tight coupling** means one class or module depends heavily on another implementation. That makes the system harder to change and test.

    **Loose coupling** means modules interact through contracts or abstractions rather than being tightly bound to specific implementations.

    NestJS promotes loose coupling through:

    - modules,
    - dependency injection,
    - service-based design,
    - provider abstraction.

    For example, a controller can depend on a `UserService` interface or a service provider instead of directly using a database implementation. This allows the underlying implementation to change without changing the controller logic.

    This modular approach makes the application easier to scale, test, and maintain over time.

    **[⬆ Back to Top](#table-of-contents)**

60. ### 60. How does NestJS support Server-Sent Events (SSE), and what are the primary advantages of using SSE for real-time communication in web applications?

    NestJS supports **Server-Sent Events (SSE)** using the `@Sse()` decorator. This allows the server to push updates to the client over a single HTTP connection without the client needing to continuously poll the server.

    Example:

    ```typescript
    @Sse('events')
    sse(): Observable<MessageEvent> {
      return interval(1000).pipe(
        map(() => ({ data: { message: 'Hello from server' } })),
      );
    }
    ```

    SSE is useful for real-time dashboards, notifications, live feeds, stock tickers, and monitoring tools. Its main advantages are simplicity, automatic reconnection, standard HTTP compatibility, and efficient one-way data streaming from server to client.

    It is ideal when the client only needs updates pushed by the server, rather than full bidirectional communication.

    **[⬆ Back to Top](#table-of-contents)**
