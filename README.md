Overview :

This project is a simple User Management System developed as a college assignment. It includes both a backend and frontend for user authentication, registration, and profile management. The backend is built using Spring Boot, and the frontend uses HTML, CSS, JavaScript, and Thymeleaf.

Features :

User Authentication: Login functionality with form validation.

User Registration: Allows users to sign up with validation for email and password.

User Profile Management: Displays user details on a profile page.

Responsive Design: Frontend is styled with Bootstrap for responsive and user-friendly design.

Secure Communication: CORS configuration is enabled to handle cross-origin requests.

Technologies Used :

Backend

Spring Boot: Framework for building the RESTful backend.

Spring Security: For authentication and authorization.

Hibernate: ORM tool for database operations.

H2 Database: In-memory database for development and testing.

Frontend

HTML: Structure of the web pages.

CSS: Styling of the web pages.

Bootstrap: Responsive design framework.

JavaScript: Client-side validation and interactivity.

Thymeleaf: Server-side rendering template engine.

Project Structure

User-Management-System/
|-- src/
|   |-- main/
|       |-- java/
|       |   |-- com/aman/authentication/
|       |       |-- controller/          # Controller classes
|       |       |-- model/               # Entity classes
|       |       |-- repository/          # Repository interfaces
|       |       |-- service/             # Service classes
|       |       |-- Application.java     # Main Spring Boot application class
|       |-- resources/
|           |-- templates/               # Thymeleaf templates (login.html, signup.html, profile.html)
|           |-- application.properties   # Application configuration
|-- static/
|   |-- css/                             # CSS files
|   |-- js/                              # JavaScript files
|-- README.md                            # Project documentation

Setup and Usage

Prerequisites

Java 21

Maven

Git

Steps to Run

Clone the repository:

git clone https://github.com/amansahugupta/UserProfile.git
cd userprofile

Build and run the application using Maven:

mvn clean install
mvn spring-boot:run

Open your browser and navigate to:

Login Page: http://localhost:8080/login

Sign-Up Page: http://localhost:8080/signup

CORS Configuration

The application allows all CORS requests for development purposes. You can modify the CORS configuration in the WebSecurityConfig.java file:

http.cors().configurationSource(request -> new CorsConfiguration().applyPermitDefaultValues());

Database Configuration

The application uses H2 Database by default. You can access the database console at:

http://localhost:8080/h2-console

Update database properties in application.properties as needed.

Frontend

The frontend templates are in the src/main/resources/templates/ directory. To customize the styles, edit the CSS files in the static/css/ directory.

Testing

Use browser developer tools to inspect network requests and ensure form validation.

Verify functionality across devices to confirm responsive design.

Folder Structure

Ensure the following folder structure is maintained for the application to function correctly:

Backend code resides in src/main/java.

Thymeleaf templates in src/main/resources/templates.

Static resources (CSS, JavaScript) in src/main/resources/static.

Contributing

Feel free to fork this repository and contribute. Submit a pull request with detailed information about your changes.

License

This project is licensed under the MIT License.
