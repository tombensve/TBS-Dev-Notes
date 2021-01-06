# ServiceLoader

Add this dependency:

```xml
    <dependen>	
	    <groupId>com.google.auto.service</groupId>
	    <artifactId>auto-service</artifactId>
	    <version>1.0-rc4</version>
	    <scope>provided</scope>
    </dependency>

```

And you can use `@AutoService(Service.class)` to automatically update META-INF/Services/...

## Example

```java
import com.google.auto.service.AutoService;

@AutoService(SimpleService.class)
public class SimpleServiceImpl implements SimpleService {
    public String echo(final String value) {
        return value;
    }
}
```

## Source

Found this on <https://itnext.io/serviceloader-the-built-in-di-framework-youve-probably-never-heard-of-1fa68a911f9b>. Indifferent from what this page says, 
ServiceLoader does not do dependencyInjection. It just looks up an implementation of a defined service.

