### Maven Project Using Command Line Project

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
* Project Build Command
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
*
