Demo code borrowed from:

- https://www.baeldung.com/jaxb
- https://stackify.com/java-xml-jackson/
- http://zetcode.com/springboot/restxml/
- https://github.com/Addicticks/jTexttime/wiki/JAXB-type-adapter-classes-for-java.time

# Links

- [Swagger UI](http://127.0.0.1:8080/swagger-ui.html)
- [OpenAPI Definition](http://127.0.0.1:8080/v2/api-docs)
- [Spring Actuator](http://127.0.0.1:8080/actuator)
- [Spring Actuator Prometheus scraper page](http://127.0.0.1:8080/actuator/prometheus)

_note: Spring Actuator endpoints are not in the swagger docs!_

# Show dependency tree

mvn dependency:tree

# Example messeges

Correct

```xml
<?xml version="1.0" encoding="UTF-8"?>
<UserResponse>
    <id>1</id>
    <name>James Denn</name>
</UserResponse>
```

Incorrect:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<UserResponse>
    <id>A</id>
    <name>James Denn</name>
</UserResponse>
```

```xml
<?xml version="1.0" encoding="UTF-8"?>
<UserResponse>
    <id>1</id>
</UserResponse>
```
