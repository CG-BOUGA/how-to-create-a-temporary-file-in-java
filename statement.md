```java runnable
// { autofold
import java.nio.file.Files;
import java.nio.file.Path;

public class Main {

public static void main(String[] args) throws Exception {

// }

String prefix = "my-application-name-";
String suffix = "";

// For files
Path file = Files.createTempFile(prefix, suffix);

// For directories
Path directory = Files.createTempDirectory(prefix);

//{ autofold

System.out.println("File created:      " + file);
System.out.println("Directory created: " + directory);

}

}
//}
```
