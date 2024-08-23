# Zeebe Worker for Camunda 8

Source code for the tutorial around Zeebe Workers written in Java.
This project contains a worker that can connect a BPMN service task.

Requirements:

* Java >= 17
* Maven

How to run:

* Download/clone the code in this folder.
* You need to set your Camunda cloud client connection details in the file `application.yaml`. Simply replace the existing sample values.
* Run the application:

```
mvn package exec:java
```

Now you need to model and deploy a BPMN process that contains a service task of type `orchestrate-something`. Start a new instance of this process instance and you will see the sysout of this worker.

- You can create a comparable worker in another programming language following one of the [Get Started Guides](https://github.com/camunda-cloud/camunda-cloud-get-started)
- This template uses the library [spring-zeebe](https://github.com/camunda-community-hub/spring-zeebe), please refer to that documentation for up to date information
- You can check the latest versions of the libraries here: https://mvnrepository.com/artifact/io.camunda.spring/spring-boot-starter-camunda and here: https://mvnrepository.com/artifact/io.camunda.spring/spring-boot-starter-camunda
