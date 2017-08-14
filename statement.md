```java runnable
// { autofold
import static java.nio.file.StandardOpenOption.APPEND;

import java.io.BufferedReader;
import java.io.BufferedWriter;
import java.io.IOException;
import java.nio.file.Files;
import java.nio.file.Path;
import java.nio.file.Paths;
import java.util.Arrays;
import java.util.List;

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
