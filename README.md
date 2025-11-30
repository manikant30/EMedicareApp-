# Medicare Project

## Description
The Medicare Project is a comprehensive healthcare management system designed to streamline the processes involved in managing patient data, appointments, and medical records. This project consists of a backend built with Java Spring Boot and a frontend developed using Angular. The system aims to provide a user-friendly interface for healthcare providers and patients, ensuring efficient management of healthcare services.

## Tech Stack
- **Backend**: Java, Spring Boot, Maven
- **Frontend**: Angular, TypeScript, HTML, CSS
- **Database**: (Assumed) MySQL or PostgreSQL
- **Testing**: JUnit for backend, Jasmine/Karma for frontend

## Folder Structure
```
medicare_project
├── medicare_backend
│   ├── .idea
│   ├── .mvn
│   ├── src
│   │   ├── main
│   │   │   ├── java
│   │   │   │   └── com
│   │   │   │       └── medicare
│   │   │   │           ├── bean
│   │   │   │           ├── controller
│   │   │   │           ├── repository
│   │   │   │           ├── service
│   │   │   │           └── MedicareBackendApplication.java
│   │   │   └── resources
│   │   └── test
│   │       ├── java
│   │       │   └── com
│   │       │       └── example
│   │       │           └── medicare_backend
│   │       │               └── MedicareBackendApplicationTests.java
│   ├── target
│   ├── .gitignore
│   ├── mvnw
│   ├── mvnw.cmd
│   └── pom.xml
├── medicare_frontend
│   ├── .angular
│   ├── .vscode
│   ├── src
│   │   ├── app
│   │   ├── assets
│   │   ├── environments
│   │   ├── favicon.ico
│   │   ├── index.html
│   │   ├── main.ts
│   │   ├── polyfills.ts
│   │   ├── styles.css
│   │   └── test.ts
│   ├── .browserslistrc
│   ├── .editorconfig
│   ├── .gitignore
│   ├── angular.json
│   ├── karma.conf.js
│   ├── package-lock.json
│   ├── package.json
│   ├── README.md
│   ├── tsconfig.app.json
│   ├── tsconfig.json
│   └── tsconfig.spec.json
└── .gitignore
```

## Dummy APIs
1. **Get All Patients**
   - **Endpoint**: `GET /api/patients`
   - **Description**: Retrieves a list of all patients in the system.

2. **Add New Patient**
   - **Endpoint**: `POST /api/patients`
   - **Description**: Adds a new patient to the system.
   - **Request Body**: 
     ```json
     {
       "name": "John Doe",
       "age": 30,
       "gender": "Male",
       "medicalHistory": "None"
     }
     ```

3. **Get Patient by ID**
   - **Endpoint**: `GET /api/patients/{id}`
   - **Description**: Retrieves details of a specific patient by ID.

4. **Update Patient**
   - **Endpoint**: `PUT /api/patients/{id}`
   - **Description**: Updates the details of an existing patient.

5. **Delete Patient**
   - **Endpoint**: `DELETE /api/patients/{id}`
   - **Description**: Deletes a patient from the system.

## How to Run the Project
### Backend
1. Navigate to the `medicare_backend` directory.
2. Run the following command to start the backend server:
   ```
   ./mvnw spring-boot:run
   ```
3. The backend will be accessible at `http://localhost:8080`.

### Frontend
1. Navigate to the `medicare_frontend` directory.
2. Install the dependencies:
   ```
   npm install
   ```
3. Start the frontend application:
   ```
   ng serve
   ```
4. The frontend will be accessible at `http://localhost:4200`.

## Screenshot
![Medicare Project Screenshot](path_to_screenshot.png)

## Conclusion
The Medicare Project is designed to enhance the efficiency of healthcare management. With a robust backend and an intuitive frontend, it aims to provide a seamless experience for users. Contributions and improvements are welcome!
