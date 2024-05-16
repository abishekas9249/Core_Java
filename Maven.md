# Maven Project Using Command Line Project

## File Structure Steps

* Download the Latest Maven Version from Maven Website
* Extract and Setup in the Environment with the following names
  * JAVA_HOME ->   C:\Program Files\Java\jdk-17
  * MAVEN_HOME ->  C:\Intel\Apache Maven 3.9.6\apache-maven-3.9.6
  * Path -> C:\Intel\Apache Maven 3.9.6\apache-maven-3.9.6 and C:\Intel\Apache Maven 3.9.6\apache-maven-3.9.6
* Run Command in Cmd Whether Maven is Available
  ```console
  mvn --version
  mvn -v
  ```
* ### Project Build Command
  ```console
  mvn archetype:generate
  ```
  ```console
  Choose a number or apply filter (format: [groupId:]artifactId, case sensitive contains): 2147: 2147
  Choose org.apache.maven.archetypes:maven-archetype-quickstart version:
  1: 1.0-alpha-1
  2: 1.0-alpha-2
  3: 1.0-alpha-3
  4: 1.0-alpha-4
  5: 1.0
  6: 1.1
  7: 1.3
  8: 1.4
  Choose a number: 8:8
  Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/archetypes/maven-archetype-quickstart/1.4/maven-archetype-quickstart-1.4.pom
  Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/archetypes/maven-archetype-quickstart/1.4/maven-archetype-quickstart-1.4.pom (1.6 kB at 52 kB/s)
  Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/archetypes/maven-archetype-bundles/1.4/maven-archetype-bundles-1.4.pom
  Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/archetypes/maven-archetype-bundles/1.4/maven-archetype-bundles-1.4.pom (4.5 kB at 144 kB/s)
  Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/archetypes/maven-archetype-quickstart/1.4/maven-archetype-quickstart-1.4.jar
  Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/archetypes/maven-archetype-quickstart/1.4/maven-archetype-quickstart-1.4.jar (7.1 kB at 284 kB/s)
  Define value for property 'groupId': com.virtusa
  Define value for property 'artifactId': DemoMavenProject
  Define value for property 'version' 1.0-SNAPSHOT: : 1.0-SNAPSHOT
  Define value for property 'package' com.virtusa: : org.virtusa
  Confirm properties configuration:
  groupId: com.virtusa
  artifactId: DemoMavenProject
  version: 1.0-SNAPSHOT
  package: org.virtusa
   Y: : Y
  [INFO] ----------------------------------------------------------------------------
  [INFO] Using following parameters for creating project from Archetype: maven-archetype-quickstart:1.4
  [INFO] ----------------------------------------------------------------------------
  [INFO] Parameter: groupId, Value: com.virtusa
  [INFO] Parameter: artifactId, Value: DemoMavenProject
  [INFO] Parameter: version, Value: 1.0-SNAPSHOT
  [INFO] Parameter: package, Value: org.virtusa
  [INFO] Parameter: packageInPathFormat, Value: org/virtusa
  [INFO] Parameter: package, Value: org.virtusa
  [INFO] Parameter: groupId, Value: com.virtusa
  [INFO] Parameter: artifactId, Value: DemoMavenProject
  [INFO] Parameter: version, Value: 1.0-SNAPSHOT
  [INFO] Project created from Archetype in dir: C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject
  [INFO] ------------------------------------------------------------------------
  [INFO] BUILD SUCCESS
  [INFO] ------------------------------------------------------------------------
  [INFO] Total time:  05:48 min
  [INFO] Finished at: 2024-05-16T13:13:03+05:30
  [INFO] ------------------------------------------------------------------------
  ```
  * ### Maven Complie Command
  ```console
  mvn compile
  [INFO] Scanning for projects...
  [INFO]
  [INFO] --------------------< com.virtusa:DemoMavenProject >--------------------
  [INFO] Building DemoMavenProject 1.0-SNAPSHOT
  [INFO]   from pom.xml
  [INFO] --------------------------------[ jar ]---------------------------------
  [INFO]
  [INFO] --- resources:3.0.2:resources (default-resources) @ DemoMavenProject ---
  [INFO] Using 'UTF-8' encoding to copy filtered resources.
  [INFO] skip non existing resourceDirectory C:\Users\abishekas\IdeaProjects\Maven   Tasks\DemoMavenProject\src\main\resources
  [INFO]
  [INFO] --- compiler:3.8.0:compile (default-compile) @ DemoMavenProject ---
  [INFO] Changes detected - recompiling the module!
  [INFO] Compiling 1 source file to C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject\target\classes
  [INFO] ------------------------------------------------------------------------
  [INFO] BUILD SUCCESS
  [INFO] ------------------------------------------------------------------------
  [INFO] Total time:  1.631 s
  [INFO] Finished at: 2024-05-16T14:12:27+05:30
  [INFO] ------------------------------------------------------------------------
  ```
* ### Maven Test Running
  ```console
  mvn test
  [INFO] Scanning for projects...
  [INFO]
  [INFO] --------------------< com.virtusa:DemoMavenProject >--------------------
  [INFO] Building DemoMavenProject 1.0-SNAPSHOT
  [INFO]   from pom.xml
  [INFO] --------------------------------[ jar ]---------------------------------
  [INFO]
  [INFO] --- resources:3.0.2:resources (default-resources) @ DemoMavenProject ---
  [INFO] Using 'UTF-8' encoding to copy filtered resources.
  [INFO] skip non existing resourceDirectory C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject\src\main\resources
  [INFO]
  [INFO] --- compiler:3.8.0:compile (default-compile) @ DemoMavenProject ---
  [INFO] Nothing to compile - all classes are up to date
  [INFO]
  [INFO] --- resources:3.0.2:testResources (default-testResources) @ DemoMavenProject ---
  [INFO] Using 'UTF-8' encoding to copy filtered resources.
  [INFO] skip non existing resourceDirectory C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject\src\test\resources
  [INFO]
  [INFO] --- compiler:3.8.0:testCompile (default-testCompile) @ DemoMavenProject ---
  [INFO] Changes detected - recompiling the module!
  [INFO] Compiling 1 source file to C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject\target\test-classes
  [INFO]
  [INFO] --- surefire:2.22.1:test (default-test) @ DemoMavenProject ---
  Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit4/2.22.1/surefire-junit4-2.22.1.pom
  Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit4/2.22.1/surefire-junit4-2.22.1.pom (3.1 kB at 7.5 kB/s)
  Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/2.22.1/surefire-providers-2.22.1.pom
  Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/2.22.1/surefire-providers-2.22.1.pom (2.5 kB at 89 kB/s)
  Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit4/2.22.1/surefire-junit4-2.22.1.jar
  Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit4/2.22.1/surefire-junit4-2.22.1.jar (85 kB at 1.3 MB/s)
  [INFO]
  [INFO] -------------------------------------------------------
  [INFO]  T E S T S
  [INFO] -------------------------------------------------------
  [INFO] Running org.virtusa.AppTest
  Welcome to Junit Testing
  [INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.065 s - in org.virtusa.AppTest
  [INFO]
  [INFO] Results:
  [INFO]
  [INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
  [INFO]
  [INFO] ------------------------------------------------------------------------
  [INFO] BUILD SUCCESS
  [INFO] ------------------------------------------------------------------------
  [INFO] Total time:  4.750 s
  [INFO] Finished at: 2024-05-16T14:16:51+05:30
  [INFO] ------------------------------------------------------------------------
  ```
* ### Maven packaging to jar file
  ```console
  mvn package
  [INFO] Scanning for projects...
  [INFO]
  [INFO] --------------------< com.virtusa:DemoMavenProject >--------------------
  [INFO] Building DemoMavenProject 1.0-SNAPSHOT
  [INFO]   from pom.xml
  [INFO] --------------------------------[ jar ]---------------------------------
  [INFO]
  [INFO] --- resources:3.0.2:resources (default-resources) @ DemoMavenProject ---
  [INFO] Using 'UTF-8' encoding to copy filtered resources.
  [INFO] skip non existing resourceDirectory C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject\src\main\resources
  [INFO]
  [INFO] --- compiler:3.8.0:compile (default-compile) @ DemoMavenProject ---
  [INFO] Nothing to compile - all classes are up to date
  [INFO]
  [INFO] --- resources:3.0.2:testResources (default-testResources) @ DemoMavenProject ---
  [INFO] Using 'UTF-8' encoding to copy filtered resources.
  [INFO] skip non existing resourceDirectory C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject\src\test\resources
  [INFO]
  [INFO] --- compiler:3.8.0:testCompile (default-testCompile) @ DemoMavenProject ---
  [INFO] Nothing to compile - all classes are up to date
  [INFO]
  [INFO] --- surefire:2.22.1:test (default-test) @ DemoMavenProject ---
  [INFO]
  [INFO] -------------------------------------------------------
  [INFO]  T E S T S
  [INFO] -------------------------------------------------------
  [INFO] Running org.virtusa.AppTest
  Welcome to Junit Testing
  [INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.053 s - in org.virtusa.AppTest
  [INFO]
  [INFO] Results:
  [INFO]
  [INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
  [INFO]
  [INFO]
  [INFO] --- jar:3.0.2:jar (default-jar) @ DemoMavenProject ---
  [INFO] Building jar: C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject\target\DemoMavenProject-1.0-SNAPSHOT.jar
  [INFO] ------------------------------------------------------------------------
  [INFO] BUILD SUCCESS
  [INFO] ------------------------------------------------------------------------
  [INFO] Total time:  3.208 s
  [INFO] Finished at: 2024-05-16T14:20:22+05:30
  [INFO] ------------------------------------------------------------------------
  ```
* ### Maven Running the Jar File After Packaging
 * #### Setting up the Jar file to Build Path  
  ```console
  set classpath=C:\Users\abishekas\IdeaProjects\Maven Tasks\DemoMavenProject\target\DemoMavenProject-1.0-SNAPSHOT.jar
  ```
 * #### Running up the Jar file 
  ```console
  java com.virtusa.App
  ```
