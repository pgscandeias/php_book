# Writing Partymapper

I'll be coding a simple backend in php, using an onion architecture for my business logic, a command pattern to expose use cases, and test-driven development throughout to ensure quality and maintainability. 

The resulting application will in many ways adhere to the principles laid out by Uncle Bob in his talk ["Architecture: the lost years"](https://www.youtube.com/watch?v=WpkDN78P884), in which he argues against tying logic to a particular web framework.

This series is written as a documentation of the thought process that goes into building a piece of software. Initial assumptions will be wrong and code will evolve, just like in real life.

Even though the series is long, most of it is about explaining concepts. After having a solid grasp of the fundamentals and some practice, writing software like this isn't necessarily slower than using an MVC framework. And in terms of maintainability, I reckon it's better.

1. [Introduction](./docs/introduction.md)
2. [Analyzing the domain](./docs/domain.md)
3. [Architecture](./docs/architecture_onion.md)
    1. [Onion](./docs/architecture_onion.md)
    2. [Command pattern](./docs/architecture_command_pattern.md)
    3. [Dependency injection](./docs/architecture_dependency_injection.md)
4. [Bootstrapping with Composer](./docs/bootstrapping.md)
5. [Writing entities](./docs/entities.md)
6. [TDD the first use case](./docs/first_use_case_tdd.md)
7. [Putting it all together with a functional test](./docs/first_use_case_functional.md)

*Work in progress*
