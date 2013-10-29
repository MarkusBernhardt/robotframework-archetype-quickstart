robotframework-archetype-quickstart
===================================

Robot Framework archetype for creating the testsuite from the quickstart guide.

Using this archetype the only thing to create a working Robot Framework 
testsuite is a existing Apache Maven installation.

Usage
-----

```bash
$ mvn -B archetype:generate \
      -DarchetypeGroupId=com.github.markusbernhardt \
      -DarchetypeArtifactId=robotframework-archetype-quickstart \
      -DarchetypeVersion=1.0.0 
      -DgroupId=mycompany.mydepartment \
      -DartifactId=myproject-mytestsuite

$ cd myproject-mytestsuite

$ mvn test
```
