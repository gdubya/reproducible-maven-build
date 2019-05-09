Simple test to prove that a maven build can be reproducible.

Comment out the reproducible-build-maven-plugin in the pom.xml to go back to default maven behaviour (non-reproducible build).

Clean build and check the md5sum of the resulting jar using the following: 
```
mvn -q clean install && md5sum target/*.jar
```