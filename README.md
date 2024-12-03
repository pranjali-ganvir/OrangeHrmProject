# OrangeHrmProject
## About The Project
[OrangeHRM application](https://opensource-demo.orangehrmlive.com/) automation testing using Selenium, TestNG, and Cucumber involves automating key HR processes like adding an employee, searching for the added employee, and deleting the account. Selenium is used for interacting with the web elements, while TestNG provides test case structuring and reporting. Cucumber is used to define test scenarios in a behavior-driven development (BDD) style.

* Adding an Employee: Automation script navigates to the "Add Employee" form, inputs necessary details, and submits.
* Searching Employee: The script searches for the newly added employee by name or ID.
* Deleting Employee: The employee record is selected and deleted, ensuring the account is removed successfully.

![Automation Demonstration](./execution.gif)

### Built With
* [Java 8](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html) as programming language
* [Maven](https://maven.apache.org/) for Package Management and Build Automation
* [Selenium](https://www.selenium.dev/) for Web Automation
* [TestNG](https://testng.org/) for Java testing framework that supports annotations, parallel execution, and detailed reporting for efficient test automation.
* [Cucumber](https://cucumber.io/docs/cucumber/) Cucumber is a testing framework that supports Behavior-Driven Development (BDD) by allowing you to write test cases in plain, human-readable language.

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites
  Basic understanding of Java with Maven, Selenium, TestNG and Cucumber.

### Running the project
Steps are listed below to get this project up and running in your development environment.

* Setup Java with JDK 1.8. For reference: Use this official [Tutorial](https://docs.oracle.com/javase/10/install/installation-jdk-and-jre-microsoft-windows-platforms.htm)

* Setup Maven. Follow this link: [Maven Setup](https://maven.apache.org/install.html)

* Clone this repository in your target folder.
```
git clone https://github.com/lavatech321/Orange_HRM_selenium_automation.git
```

* Open _orange_hrm.automation_ folder in Eclipse by selecting "File -> Import -> Maven -> Existing Maven Project" and select _orange_hrm.automation_ folder. 
  
Optionally, run maven build command if you don't see "Maven Dependencies" folder:

```
mvn clean install
```

You can also right click the project, and select "Maven -> Update Project -> Check the 'Force Update of Snapshots/Releases' -> Ok". This will update the "Maven Dependencies" project.

* Open _orange_hrm.automation_ folder in Eclipse by selecting "File -> Import -> Maven -> Existing Maven Project" and select _orange_hrm.automation_ folder. 
  
* Execute the project using below maven command:

```
mvn clean test
```

* Optionally, after making any changes to the repository, you can package the code into a jar file:
  
```
mvn clean package
```
  
_Note: I have used JAR for packaging. If you want to build into the jar file, change the `<packaging>` inside pom.xml file to war._

```
 <packaging>jar</packaging>
```

Congrats !!! You are now able to run the project in your own development environment.

* You can run this project as _TestNG Suite_ by right clicking the project and select "Run As -> TestNG Suite".

_Note: I have place *testng.xml* file under src/test/resources folder._

