# HR Job Management API

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)

This is a Spring Boot application that allows for the management of Human Resources (HR) job openings.

## Requirements

- Java 17 or higher
- Maven
- Database (Postgres)

## Configuration

1. Clone the repository:

   ```shell
   git clone https://github.com/cmtavares/job-management.git
   ```

2. Configure the database by editing the application.properties file and providing the necessary settings:

    ```properties
    spring.datasource.url=jdbc:postgresql://localhost:5432/database
    spring.datasource.username=admin
    spring.datasource.password=admin
    ```

3. Build the application:

    ```shell
    mvn clean install
    ```

4. Start the application:

    ```shell
    mvn spring-boot:run
    ```

The application should now be running at http://localhost:8080.


## Documentation:
Access the complete API documentation for detailed information on the endpoints and how to use them <a href="https://documenter.getpostman.com/view/32463762/2sA3XV8enz">here</a>.



## EndPoints

#### Create Candidate
```shell
curl --location --request POST 'http://localhost:8080/candidate/' \
--header 'Content-Type: application/json' \
--data-raw '{
    "username": "jose",
    "name": "Jose de Souza",
    "email": "jose@gmail.com",
    "password": "1234567890",
    "description": "Junior Java Developer looking for the first opportunity."
}'
```
