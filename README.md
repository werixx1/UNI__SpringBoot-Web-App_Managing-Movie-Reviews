
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring MVC](https://img.shields.io/badge/Spring_MVC-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=thymeleaf&logoColor=white)
![H2 Database](https://img.shields.io/badge/H2_Database-09476B?style=for-the-badge&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)

# UNI__SpringBoot-Web-App_Managing-Movie-Reviews
A simple web application for managing movies, movie reviews and users using the Springboot framework. Project has been developed for web technologies course.
> Compsci course: Second year, second semester

## Features

- implemented simple website ui using thymeleaf that allows the user to view, add, edit and delete resources using the browser (forms, buttons, etc.). via localhost   
-  implemented REST API that enables programmatic access to the same data (by using Postman for example) and performing all basic http operations (GET, POST, PUT, DELETE)  
- implemented a set of custom REST endpoints for data analytics and reports
- in-memory H2 database support

## Example of usage

https://github.com/user-attachments/assets/dfda8174-71c8-402e-b520-113660014bbc
  
## Custom REST endpoints:

```
api/movies/title/{movieTitle} <- get movie by title
api/movies/genre/{genre} <- get movies by genre
api/movies/best-rated-movie/genre/{genre} <- get best rated movie
api/movies/worst-rated-movie/genre/{genre} <- get worst rated movie
api/movies/movie-with-most-reviews <- get movie with most reviews added
```
```
api/reviews/user/{userId} <- get all reviews of user
api/reviews/movie/id/{movieId} <- get reviews for certain movie (by its id)
api/reviews/latest-review <- get newest review
```
 ```
api/users/username/{username} <- get user by username
api/users/user-with-most-reviews <- get user with most reviews posted
api/users/inactive-users <- get inactive users
```
```
api/database/raport <- get info about number of users, reviews, movies in the database and how many movies are for each genre
```

### Examples
Movies |  Users/inactive users
:-------------------------:|:-------------------------:
![obraz](https://github.com/user-attachments/assets/8784672c-0fec-432b-a1f0-d05bbe0616a0) |  ![obraz](https://github.com/user-attachments/assets/dcc85bfc-6877-41b8-b2bd-d6db1e70ab5b)

## Project Structure

```
SpringBoot-web-app-for-managing-movie-reviews/
│
├── src/
│   ├── main/
│   │   ├── java/com/example/
│   │   │   └── reviewsmanager/
│   │   │       ├── controller/    # Handles web requests and API endpoints
│   │   │       ├── service/       # Contains business logic
│   │   │       ├── repository/    # Handles database operations
│   │   │       ├── model/         # Defines application data entities
│   │   │       ├── dto/           # Transfers data between application layers
│   │   │       └── ReviewsManagerApplication.java   # Starts the Spring Boot application
│   │   │
│   │   └── resources/
│   │       ├── templates/         # HTML pages rendered with Thymeleaf
│   │       └── application.properties  # Application configuration
│   │
│   └── test/
│       └── java/                  # Automated tests (not applied)
│
├── .mvn/
│   └── wrapper/                   # Maven Wrapper configuration
│
├── pom.xml                        # Dependencies and build configuration
├── mvnw                           # Maven Wrapper for Linux/macOS
├── mvnw.cmd                       # Maven Wrapper for Windows
├── README.md                      # Project documentation
└── .gitignore                     # Files excluded from Git
```
## Helpful resources for understanding springboot:
- [CRUD](https://www.youtube.com/watch?v=7nonQ2dYgiE)
- [CRUD](https://www.youtube.com/watch?v=ZZTYQIUd_uY)
- [Queries](https://www.youtube.com/watch?v=eSaXN7WqQKI)
- [Spring Data JPA Query Methods](https://docs.spring.io/spring-data/jpa/reference/jpa/query-methods.html)
- [DTO](https://www.youtube.com/watch?v=MAIkC9KctVw)
- [Thymeleaf](https://www.youtube.com/watch?v=MUhDe_yZ5WQ)
   
## License

This project is distributed under the MIT license.

