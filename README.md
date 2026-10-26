# Functional Programming Demo (No Stream)

A Java-based learning project that demonstrates the core ideas of functional programming using lambda expressions, custom functional interfaces, and Java's built-in functional APIs. The app models a simple `Person` dataset and shows how to filter, transform, sort, and process data in a functional style.

## Overview

This project is intended as a practical, beginner-friendly example of functional programming in Java. It focuses on the foundational concepts that make Java code more expressive, reusable, and declarative:

- Lambda expressions
- Functional interfaces
- Predicates and composition
- Consumers and actions
- Stream-based collection processing
- Data transformation and filtering

## Features

- Simple `Person` domain model with name, age, city, and active status
- Custom functional interfaces:
  - `PersonRule`
  - `PersonAction`
- Java standard functional interfaces:
  - `Predicate<Person>`
  - `Consumer<Person>`
- Stream operations for:
  - filtering
  - counting
  - sorting
  - mapping
  - distinct selection
  - optional value retrieval
- Predicate composition using `and()`, `or()`, and `negate()`

## Project Structure

```text
functional-programming-nostream/
├── pom.xml
├── src/
│   └── main/
│       └── java/
│           └── com/
│               └── gloriane/
│                   ├── Main.java
│                   ├── Person.java
│                   ├── PersonAction.java
│                   ├── PersonRule.java
│                   └── PersonProcessor.java
├── .gitignore
└── README.md
```

## Tech Stack

- Java 25
- Maven
- Functional programming patterns in Java SE

## Prerequisites

Before running this project, ensure your environment includes:

- Java 25 or higher
- Maven installed and available in your PATH

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Gloriane7767/functional-programming-nostream.git
cd functional-programming-nostream
```

### 2. Compile the project

```bash
mvn clean compile
```

### 3. Run the application

```bash
java -cp target/classes com.gloriane.Main
```

## What the App Demonstrates

The program creates a list of sample people and applies functional techniques to:

- find active people
- count adults
- sort people by age
- locate the first active person in a given city
- combine predicates logically
- collect unique city names
- extract initials from names
- format strings from object data
- generate example email addresses
- perform actions on matching records with `Consumer`

## Example Behavior

The app prints several sections of output, including:

```text
=== PREDICATE & CONSUMER SECTION ===

Active people: [Person{...}, ...]
Adult count: 5
Sorted by age: [Person{...}, ...]
First active in Stockholm: Optional[Person{...}]
Active adults: [...]
Adults or in Stockholm: [...]
Inactive people: [...]
Cities: [Gothenburg, Malmö, Stockholm, Uppsala]
First letters: [A, E, L, N, O, S]
Formatted: [...]
Email list: [...]
```

## Learning Goals

This project is well-suited for:

- learning Java lambdas
- understanding functional interfaces
- exploring `Predicate`, `Consumer`, and stream pipelines
- practicing declarative data processing
- building confidence in functional-style Java code

## License

This project does not currently include a license file. If you plan to share or distribute it publicly, consider adding a license such as MIT or Apache 2.0.

## Repository

- GitHub: https://github.com/Gloriane7767/functional-programming-nostream

## Author

Gloriane7767
