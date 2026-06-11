# fz-spring-boot-starter-dependencies

Spring Boot Starter 依赖版本管理项目。

## 项目简介

这是一个 Spring Boot Starter 依赖管理项目，用于统一管理项目中所有 Spring Boot Starter 的依赖版本。通过使用该项目，可以简化子模块的依赖配置，避免版本冲突。

## 主要功能

- 统一管理 Spring Boot 相关依赖版本
- 提供 BOM (Bill of Materials) 配置
- 简化子模块的依赖引入

## 使用方法

在 Maven 项目的 `pom.xml` 中继承此项目：

```xml
<parent>
    <groupId>com.xxx</groupId>
    <artifactId>fz-spring-boot-starter-dependencies</artifactId>
    <version>x.x.x</version>
</parent>
```

或引入依赖管理：

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

## 技术栈

- Java
- Maven
- Spring Boot

## 版本要求

- JDK 1.8+

## 许可证

本项目基于 [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0) 许可证开源。