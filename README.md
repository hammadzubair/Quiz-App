
# Quiz App

Quiz application is Java Web Application, developed on springboot,hibernate,maven with thymleaf, can be use for the assessment of student by the lecturer during lecture.

### **How to build the application**
The build system is used in this application is Maven, Following are the steps to build this application
- Clone the repository into your IDE, I used IntelliJ IDEA.
- You will see Maven module up right sidebar of IDE.
- If you didn't get maven module, go to View -> Tool Windows -> and select Maven.
- Now in Maven module expand **Lifecycle** and click on **clean**.
- After Clean click on  **install**
- You will  get **BUILD SUCCESS** message in your terminal window and **Quiz-Application.jar** in the  **target** folder of the project directory.

### **How to deploy the application**
-Open project in explorer and open command prompt or go to your start menu and run cmd as administrator and move on to project directory.
- write command **docker-compose build**
- After that write command **docker-compose up**
-  Make sure ports 8080 and 3306 are free to use as the applcation will deploy on port 8080 with database  3306
- Go to browser and type  in url: http://localhost:8080/
- The application will start running

### **Architecture**
The architecture of the web application is Monolithic and Three Tier (Three Layer) Architecture in which each layer communicates with the layer directly below or above (hierarchical structure) build  with the following components:

**Presentation layer:** This is the user interface of the application that presents the application's features and data to the user.

**Business logic (or Application) layer:** This layer contains the business logic that drives the application's core functionalities. Like making decisions, calculations, evaluations, and processing the data passing between the other two layers.

**Data access layer (or Data) layer:** This layer is responsible for interacting with databases to save and retrieve application data.

#### Example
1. Spring MVC controller receives an HTTP request from the client ( browser).
2. Spring MVC controller process the request and sends that request to the service layer.
3. Service Layer responsible to hold the business logic of the application.
4. Repository layer responsible for interacting with databases to save and retrieve application data.
5. Spring MVC controller return view on Thymeleaf to render on the browser.
