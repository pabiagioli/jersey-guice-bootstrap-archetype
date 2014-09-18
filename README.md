jersey-guice-webapp-archetype
================================

Maven Archetype for building RESTful Web Services with Jersey 1.18.1 and Guice 3

Dependencies
------------
- Servlet 2.5
- Jersey 1.18.1
- Guice 3.0
- guice-persist 3.0
- gson 2.2.4
- joda-time 2.4
- JUnit 4.10

Requirements
------------
- Java 7
- Maven 3
- Tomcat 7

Install and Generate a Project
-------------------------------
```bash
#!/bin/bash
### Install the Archetype in your local Maven Repo 
mvn install
### Create a New Maven Project from command line:
mvn archetype:generate -DarchetypeGroupId=com.pampanet \
  -DarchetypeArtifactId=jersey-guice-webapp-archetype \
  -DarchetypeVersion=0.1.0-RELEASE \
  -DgroupId=<my.company.name> \
  -DartifactId=<sample> \
  -DarchetypeRepository=local \
  -DinteractiveMode=false
```

Security Frameworks
--------------------
- If you're more interested in a secured RESTful WebApp try my other archetype which integrates Apache Shiro
- https://github.com/pabiagioli/secure-rest-webapp-archetype