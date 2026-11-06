# Spring Boot Shop

A Java e-commerce learning project with a product catalog, customer registration, cart management, and an admin area for products, categories, and customers.

Built with Java 11, Spring Boot 2.6, Spring MVC, JSP, Hibernate, Spring Security, and MySQL.

## Run locally

You need Java 11 and MySQL. Run the application from `JtProject/` so the JSP views resolve correctly.

1. Configure `db.url`, `db.username`, and `db.password` in [application.properties](JtProject/src/main/resources/application.properties) for your local database.
2. Import [basedata.sql](JtProject/basedata.sql) if you want sample categories, products, and accounts.
3. Start the application:

```sh
cd JtProject
./mvnw spring-boot:run
```

On Windows, use `.\mvnw.cmd spring-boot:run`. Open http://localhost:8080.

The sample SQL creates local demonstration accounts: `admin / 123` and `lisa / 765`. These credentials are for disposable local development only.

## Structure

| Path | Purpose |
| --- | --- |
| `controller/` | Customer and admin routes |
| `models/` | Products, categories, customers, and carts |
| `dao/` | Database access |
| `services/` | Application services |
| `src/main/webapp/views/` | JSP pages |

Java packages are under `JtProject/src/main/java/com/jtspringproject/JtSpringProject/`.

## Development status

This is a learning project using an older Spring Boot stack. Cart behavior, authentication, and deployment configuration need review before production use. No payment integration is included.

Run the existing test suite from `JtProject/` with `./mvnw test`; database configuration may be required.

## Acknowledgment

Based on [jaygajera17/E-commerce-project-springBoot](https://github.com/jaygajera17/E-commerce-project-springBoot), as referenced in the original project documentation.
