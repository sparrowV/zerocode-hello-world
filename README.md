Zerocode Hello World
===

#### How to run the examples?
Ans: The same and usual stuff you do everyday for any maven project.

Step-1: 
* Import this maven project `zerocode-hello-world` using Eclipse or IntelliJ or your favourite IDE
```
          * i.e. /zerocode-hello-world/pom.xml, 
          * mvn clean install -DskipTests
          * The above command brings all the libs to the local .m2 repo
```

Step-2:
* Run the JustHelloWorldTest.java test (it invokes GitHub REST https apis and asserts the result)
```
          * i.e. src/test/java/org/jsmart/zerocode/testhelp/tests/helloworld/JustHelloWorldTest.java
          * Then fiddle with the assertions section and run the test again, observe the PASS/FAILURES at the console.
          
          * To run more tests go to individual package and run. e.g. folders-  helloworldgithub, helloworldmore etc
```
Done.
That's it. It is as simple as that.

---


So when your tests grows to **thousands** in numbers, you need to organize them by feature, by consumer and/or by profile etc. Hence Zerocode helps here to maintain peace! 

Also it **saves** you from creating thousands of java `Pojos` and getting lost in `interpreting` actual request/response.

Step-3: (Optional Step to bring up **local REST server** and fiddle with the tests)
```
Start the Local Mock REST server
          * i.e. just Run as main() -> test/.../RunMeFirstRESTServer.java. 
          * Then you can run the src/test/java/org/jsmart/zerocode/testhelp/tests/helloworldmore/JustHelloWorldMoreTest.java
```

Run as Suite:
```
          * src/test/java/org/jsmart/zerocode/testhelp/tests/HelloWorldGitHubSuite.java

More examples:
          * src/test/java/org/jsmart/zerocode/testhelp/tests/helloworldmore/JustHelloWorldMoreTest.java
          * -or- Browse under test/resources/ folders- helloworld, helloworld_github_REST_api, helloworld_more
```
Done.

Now you can see the-
* Reports @ `target`
* Logs @ `target/logs/zerocode_test_logs.log`
* Test coverage CSV Report @ `target/zerocode_full_report_YYYY-MM-DDTHH-MM-SS.SSS.csv`
* Test coverage Chart @ `target/zerocode_results_chart_YYYY-MM-DDTHH-MM-SS.SSS.html`
* More [reports](https://github.com/authorjapps/zerocode#generated-reports-and-charts)

References:
---
Eclipse(General key-board shotcuts):
=====
For quick reference only- See more eclipse keys https://www.linkedin.com/pulse/top-30-eclipse-keyboard-shortcuts-java-programmer-jayveersinh-solanki/
1. Open a matching java file -> Ctrl + Shift + R
1. Open a matching JSON file -> Ctrl + Shift + R
1. To navigate to file -> Ctrl + Click

IntelliJ(General key-board shotcuts):
=====
More keys: https://www.jetbrains.com/help/idea/mastering-intellij-idea-keyboard-shortcuts.html
1. Open a matching java file -> Ctrl + n
1. Open a matching JSON or XML file -> Ctrl + Shift + n
1. To navigate to file -> Ctrl + Click

