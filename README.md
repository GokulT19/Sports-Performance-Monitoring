# Sports Performance Monitoring

This Spring Boot application provides a platform for athletes, coaches, and administrators to manage sports performance and event participation.

**Features:**

* **Athlete Features:**
    * Register for events
    * Request coaching assistance
    * View event details
    * Communicate directly with coaches (new feature)
* **Coach Features:**
    * Accept or reject athlete requests
    * Communicate directly with athletes (new feature)
* **Administrator Features:**
    * Create events
    * Manage registrations
    * Publish results

**Technology Stack:**

* Spring Boot
* MySQL
* JWT (JSON Web Token) for authentication
* Spring Security for authorization
* HTML, CSS, and JavaScript for the frontend

**Dependencies:**

```xml
<dependencies>
    <dependency>
       <groupId>org.springframework.boot</groupId>
       <artifactId>spring-boot-starter-data-jpa</artifactId>
    </dependency>
    <dependency>
       <groupId>org.springframework.boot</groupId>
       <artifactId>spring-boot-starter-security</artifactId>
    </dependency>
    <dependency>
       <groupId>org.springframework.boot</groupId>
       <artifactId>spring-boot-starter-validation</artifactId>
    </dependency>
    <dependency>
       <groupId>org.springframework.boot</groupId>
       <artifactId>spring-boot-starter-web</artifactId>
    </dependency>

    <dependency>
       <groupId>com.mysql</groupId>
       <artifactId>mysql-connector-j</artifactId>
       <scope>runtime</scope>
    </dependency>
    <dependency>
       <groupId>org.springframework.boot</groupId>
       <artifactId>spring-boot-starter-test</artifactId>
       <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>io.jsonwebtoken</groupId>
        <artifactId>jjwt-api</artifactId>
        <version>0.11.5</version> </dependency>
    <dependency>
       <groupId>io.jsonwebtoken</groupId>
       <artifactId>jjwt-impl</artifactId>
       <version>0.11.5</version>
       <scope>runtime</scope>
    </dependency>
    <dependency>
       <groupId>io.jsonwebtoken</groupId>
       <artifactId>jjwt-jackson</artifactId> 
       <version>0.11.5</version>
       <scope>runtime</scope>
    </dependency>
    <dependency>
       <groupId>org.springframework.security</groupId>
       <artifactId>spring-security-test</artifactId>
       <scope>test</scope>
    </dependency>
    <dependency>
       <groupId>jakarta.persistence</groupId>
       <artifactId>jakarta.persistence-api</artifactId>
       <version>3.1.0</version> </dependency>
       <dependency>
           <groupId>org.projectlombok</groupId>
           <artifactId>lombok</artifactId>
           <scope>provided</scope>
       </dependency>

   </dependencies>

Configuration:

Application Properties:

spring.datasource.username: [Your MySQL username]
spring.datasource.password: [Your MySQL password]
spring.datasource.url: jdbc:mysql://localhost:3306/SportsManagement?createDatabaseIfNotExist=true&useSSL=false&allowPublicKeyRetrieval=true1
Note: Replace SportsManagement with your actual database name if different.
  
1.
github.com
MIT
github.com
You can find detailed configuration properties in the application.properties file.

Getting Started:

Clone the repository:

Bash

git clone <repository_url> 
Build the project:

Bash

mvn clean install 
Configure database credentials:

Open the application.properties file.
Replace the placeholder values for spring.datasource.username and spring.datasource.password with your actual MySQL credentials.
If you use a different database name, update the spring.datasource.url accordingly.
Run the application:

Bash

mvn spring-boot:run 
Contact:

For any questions or feedback, please contact Gokul Thakral at gokulthakral@gmail.com.


This version incorporates the following improvements:

* **Added "Clone the repository" and "Build the project" steps** to the "Getting Started" section for clarity.
* **Included a reminder to update the database name** if it differs from the default in the `application.properties` file.
* **Minor formatting adjustments** for better readability.

This README file now provides a comprehensive and user-friendly guide for setting up and running the Sports Performance Monitoring application.
