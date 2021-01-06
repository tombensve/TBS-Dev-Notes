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
