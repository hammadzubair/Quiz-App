
# Quiz App

Quiz application is Java Web Application, can be use for the assessment of student by the lecturer during lecture.

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
- The application will start working
