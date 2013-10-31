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
      -DarchetypeVersion=1.0.1 \
      -DgroupId=com.yourcompany.yourdepartment \
      -DartifactId=yourproject-yourtestsuite

$ cd yourproject-yourtestsuite

$ mvn test

[INFO]
[INFO] --- robotframework-maven-plugin:1.2:run (test) @ yourproject-yourtestsuite ---
==============================================================================
Robotframework
==============================================================================
Robotframework.Quickstart
==============================================================================
Robotframework.Quickstart.Quickstart :: Robot Framework is a keyword-driven...
==============================================================================
User can create an account and log in                                 | PASS |
------------------------------------------------------------------------------
User cannot log in with bad password                                  | PASS |
------------------------------------------------------------------------------
User can change password                                              | PASS |
------------------------------------------------------------------------------
User status is stored in database                                     | PASS |
------------------------------------------------------------------------------
Too short password                                                    | PASS |
------------------------------------------------------------------------------
Too long password                                                     | PASS |
------------------------------------------------------------------------------
Password without lowercase letters                                    | PASS |
------------------------------------------------------------------------------
Password without capital letters                                      | PASS |
------------------------------------------------------------------------------
Password without numbers                                              | PASS |
------------------------------------------------------------------------------
Password with special characters                                      | PASS |
------------------------------------------------------------------------------
Robotframework.Quickstart.Quickstart :: Robot Framework is a keywo... | PASS |
10 critical tests, 10 passed, 0 failed
10 tests total, 10 passed, 0 failed
==============================================================================
Robotframework.Quickstart                                             | PASS |
10 critical tests, 10 passed, 0 failed
10 tests total, 10 passed, 0 failed
==============================================================================
Robotframework                                                        | PASS |
10 critical tests, 10 passed, 0 failed
10 tests total, 10 passed, 0 failed
==============================================================================
Output:  /yourproject-yourtestsuite/target/robotframework-reports/output.xml
XUnit:   /yourproject-yourtestsuite/target/robotframework-reports/TEST-robotframework.xml
Log:     /yourproject-yourtestsuite/target/robotframework-reports/log.html
Report:  /yourproject-yourtestsuite/target/robotframework-reports/report.html
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------

```
