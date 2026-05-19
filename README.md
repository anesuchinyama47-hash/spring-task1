Spring Boot Task 1 – Simple Web Application

Project Description

This project is a simple Spring Boot web application created as part of Task 1.

It demonstrates:
•	Creating a Spring Boot project
•	Handling HTTP requests
•	Using a controller
•	Returning plain text with @ResponseBody
•	Rendering a view using Thymeleaf (MVC pattern)
 
 Technologies Used
•	Java
•	Spring Boot
•	Spring Web
•	Thymeleaf
•	Maven
•	IntelliJ IDEA
 
How to Run the Application
1.	Open the project in IntelliJ IDEA
2.	Wait for Maven dependencies to load
3.	Run the main class:
4.	DemoApplication.java
5.	Wait until you see:
6.	Tomcat started on port 8080
 
 Available Endpoints
1. Root endpoint (simple response)
URL:
http://localhost:8080/
Description:
•	Returns a simple text message using @ResponseBody
Response:
Hello Spring!
 
2. Greeting page (Thymeleaf view)
URL:
http://localhost:8080/greeting
Description:
•	Uses Spring MVC pattern
•	Returns an HTML page
•	Displays a message and an image
 
Project Structure
src
 └── main
     ├── java/com/example/demo
     │    ├── DemoApplication.java
     │    └── controller
     │         └── HelloController.java
     │
     └── resources
          ├── templates
          │     └── greeting.html
          └── static
                └── vistula.png
 
Key Concepts Explained
🔹 @RestController vs @Controller
•	@RestController → returns data (text/JSON)
•	@Controller → returns HTML views
 
🔹 @GetMapping
•	Maps HTTP GET requests to a method
Example:
@GetMapping("/greeting")
 
🔹 @ResponseBody
•	Returns raw response (text) instead of HTML
 
🔹 Thymeleaf
•	Template engine used to render HTML
Example:
<h1 th:text="${message}"></h1>
 
2. Greeting page with image
 
 
Features Implemented
✔ Spring Boot project created
✔ Controller implemented
✔ HTTP request handling
✔ Use of @ResponseBody
✔ Thymeleaf view rendering
✔ Static resources (image)
 
 Notes
•	Application runs on default port 8080
•	Image must be placed in:
•	src/main/resources/static
 
 Author
Anesu Chinyama 74851


