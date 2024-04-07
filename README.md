# Quiz Application

Welcome to the Quiz Application! This application allows users to take quizzes in various categories and receive personalized certificates based on their performance.

## Features

- **User Authentication**: Implemented JWT token authentication for secure user login and data protection.
- **Dynamic Quiz Categories**: Users can choose from a variety of quiz categories tailored to their interests.
- **Interactive Quiz Experience**: Engage users with dynamic quiz questions presented based on their selected category.
- **Email Integration**: Integrated email functionality to send login credentials and quiz results to users.
- **Certificate Generation**: Automatically generate personalized certificates for users based on their quiz performance.

## Technologies Used

- **Frontend**:
  - React.js
  - HTML
  - CSS

- **Backend**:
  - Spring Boot
  - Java

- **Database**:
  - MySQL

- **Authentication**:
  - JWT (JSON Web Tokens)

## Steps To Run Application Frontend

1. Clone the repository:
   ```bash
   git clone https://github.com/Saurav-Gheewala/Quiz-Application.git
   ```
2. Open the code of frontend folder in your preferred IDE like VS Code.
3. Make sure that your command prompt navigated to your frontend directory if not navigate to the project directory:
    ```bash
    cd quiz-application
    ```
4. Install dependencies:
    ```bash
    npm i
    ```
5. Run the application:
    ```bash
    npm run dev
    ```
6. Access the application in your web browser at http://localhost:5178.

## Steps To Run Application Backend

1. If you already cloned my depository then we follow the given steps if not, first cloned the repository by given command:
 ```bash
   git clone https://github.com/Saurav-Gheewala/Quiz-Application.git
   ```
2. Open the code of backend folder in your preferred IDE like intelliJ IDEA
3. Configure given code in your application properties in resource folder.
    ```bash
    server.port=8080
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    spring.datasource.url= *Database URL
    spring.datasource.username= *Database Username
    spring.datasource.password= *Database Password
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect

    spring.mail.host=smtp.gmail.com
    spring.mail.port=587
    spring.mail.username= *Your Email Id
    spring.mail.password= *Application Password Of Your Email ID
    spring.mail.properties.mail.smtp.auth=true
    spring.mail.properties.mail.smtp.starttls.enable=true
    ```
4. Make sure that you apply all the given dependencies in your porm.xml file.
    Dependencies:
    ```bash
    <dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-data-jpa</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-mail</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-mail</artifactId>
		</dependency>
		<!-- https://mvnrepository.com/artifact/org.apache.commons/commons-csv -->
		<dependency>
			<groupId>org.apache.commons</groupId>
			<artifactId>commons-csv</artifactId>
			<version>1.10.0</version>
		</dependency>

		<dependency>
			<groupId>com.mysql</groupId>
			<artifactId>mysql-connector-j</artifactId>
			<scope>runtime</scope>
		</dependency>
		<dependency>
			<groupId>org.projectlombok</groupId>
			<artifactId>lombok</artifactId>
			<optional>true</optional>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
		</dependency>
	</dependencies>
    ```
5. Run the project, it will run on 
    ```bash
    http://localhost:8080/
    ```
6. you have to provide APIs through http://localhost:8080/.
## Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

    1.  Fork the repository.
    2. Create a new branch for your feature or bug fix.
    3. Make your changes and commit them.
    4. Push to your fork and submit a pull request.
