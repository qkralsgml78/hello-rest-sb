# hello rest spring boot

### TEST
```
$ ./gradlew clean

BUILD SUCCESSFUL in 622ms
1 actionable task: 1 executed
$ ls -l build/
ls: cannot access 'build/': No such file or directory
$ ./gradlew test

> Task :test
OpenJDK 64-Bit Server VM warning: Sharing is only supported for boot loader classes because bootstrap classpath has been appended

GreetingControllerTests > noParamGreetingShouldReturnDefaultMessage() FAILED
    java.lang.AssertionError at GreetingControllerTests.java:40

GreetingControllerTests > paramGreetingShouldReturnTailoredMessage() FAILED
    java.lang.AssertionError at GreetingControllerTests.java:48

2 tests completed, 2 failed

> Task :test FAILED

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':test'.
> There were failing tests. See the report at: file:///home/nori/code/hello-rest-sb/build/reports/tests/test/index.html

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights.

* Get more help at https://help.gradle.org

BUILD FAILED in 3s
3 actionable tasks: 3 executed
$ ./gradlew jar

BUILD SUCCESSFUL in 817ms
2 actionable tasks: 1 executed, 1 up-to-date
$ ./gradlew bootJar

BUILD SUCCESSFUL in 929ms
3 actionable tasks: 2 executed, 1 up-to-date
$ ls -lh build/libs
total 19M
-rw-r--r-- 1 nori nori 2.8K Feb 27 15:41 rest-service-0.0.1-SNAPSHOT-plain.jar
-rw-r--r-- 1 nori nori  19M Feb 27 15:41 rest-service-0.0.1-SNAPSHOT.jar
$ ./gradlew clean build

> Task :test
OpenJDK 64-Bit Server VM warning: Sharing is only supported for boot loader classes because bootstrap classpath has been appended

GreetingControllerTests > noParamGreetingShouldReturnDefaultMessage() FAILED
    java.lang.AssertionError at GreetingControllerTests.java:40

GreetingControllerTests > paramGreetingShouldReturnTailoredMessage() FAILED
    java.lang.AssertionError at GreetingControllerTests.java:48

2 tests completed, 2 failed

> Task :test FAILED

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':test'.
> There were failing tests. See the report at: file:///home/nori/code/hello-rest-sb/build/reports/tests/test/index.html

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights.

* Get more help at https://help.gradle.org

BUILD FAILED in 3s
7 actionable tasks: 7 executed
```

### BUILD
```
```

### RUN
```
```
