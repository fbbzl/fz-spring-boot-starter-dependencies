# fz-spring-boot-starter-dependencies

A Spring Boot Starter dependency version management project.

## Project Overview

This is a dependency management project for Spring Boot Starters, designed to unify the version management of all Spring Boot Starter dependencies within a project. By using this project, you can simplify dependency configuration in submodules and avoid version conflicts.

## Key Features

- Unified management of Spring Boot-related dependency versions
- Provides BOM (Bill of Materials) configuration
- Simplifies dependency inclusion in submodules

## Usage

Inherit this project in your Maven project's `pom.xml`:

```xml
<parent>
    <groupId>com.xxx</groupId>
    <artifactId>fz-spring-boot-starter-dependencies</artifactId>
    <version>x.x.x</version>
</parent>
```

Or import dependency management:

```xml
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>com.xxx</groupId>
            <artifactId>fz-spring-boot-starter-xxx</artifactId>
            <version>x.x.x</version>
        </dependency>
    </dependencies>
</dependencyManagement>
```

## Technology Stack

- Java
- Maven
- Spring Boot

## Version Requirements

- JDK 1.8+

## License

This project is open-source under the [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).