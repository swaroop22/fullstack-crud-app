# fullstack-crud-app
Full Stack Java CRUD Application with Spring Boot backend and React frontend

## 📋 Project Overview

This is a Full Stack CRUD (Create, Read, Update, Delete) application built with:
- **Backend**: Java Spring Boot, Spring Data JPA, MySQL
- **Frontend**: React.js with Axios for API calls
- **Architecture**: RESTful API design

## 🏗️ Project Structure

```
fullstack-crud-app/
├── backend/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── fullstack/
│   │   │   │           └── crud/
│   │   │   │               ├── FullstackCrudApplication.java
│   │   │   │               ├── controller/
│   │   │   │               │   └── EmployeeController.java
│   │   │   │               ├── model/
│   │   │   │               │   └── Employee.java
│   │   │   │               ├── repository/
│   │   │   │               │   └── EmployeeRepository.java
│   │   │   │               ├── service/
│   │   │   │               │   └── EmployeeService.java
│   │   │   │               └── exception/
│   │   │   │                   └── ResourceNotFoundException.java
│   │   │   └── resources/
│   │   │       └── application.properties
│   │   └── test/
│   └── pom.xml
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── AddEmployee.js
│   │   │   ├── EmployeeList.js
│   │   │   ├── UpdateEmployee.js
│   │   │   └── ViewEmployee.js
│   │   ├── services/
│   │   │   └── EmployeeService.js
│   │   ├── App.js
│   │   ├── App.css
│   │   └── index.js
│   └── package.json
└── README.md
```

## 🚀 Features

- ✅ Create new employee records
- ✅ View all employees in a list
- ✅ View individual employee details
- ✅ Update employee information
- ✅ Delete employee records
- ✅ RESTful API endpoints
- ✅ Responsive UI design
- ✅ Form validation

## 🛠️ Technologies Used

### Backend
- Java 17+
- Spring Boot 3.x
- Spring Data JPA
- Spring Web
- MySQL Database
- Maven
- Lombok

### Frontend
- React.js 18+
- Axios
- React Router DOM
- Bootstrap 5
- CSS3

## 📦 Prerequisites

- Java JDK 17 or higher
- Node.js 16+ and npm
- MySQL 8.0+
- Maven 3.6+
- Git

## ⚙️ Backend Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/swaroop22/fullstack-crud-app.git
   cd fullstack-crud-app
   ```

2. **Configure MySQL Database**
   - Create a database named `employee_db`
   ```sql
   CREATE DATABASE employee_db;
   ```

3. **Update application.properties**
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/employee_db
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.show-sql=true
   ```

4. **Build and run the backend**
   ```bash
   cd backend
   mvn clean install
   mvn spring-boot:run
   ```
   Backend will run on `http://localhost:8080`

## 🎨 Frontend Setup

1. **Navigate to frontend directory**
   ```bash
   cd frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```
   Frontend will run on `http://localhost:3000`

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/v1/employees` | Get all employees |
| GET | `/api/v1/employees/{id}` | Get employee by ID |
| POST | `/api/v1/employees` | Create new employee |
| PUT | `/api/v1/employees/{id}` | Update employee |
| DELETE | `/api/v1/employees/{id}` | Delete employee |

## 📝 Sample Employee JSON

```json
{
  "firstName": "John",
  "lastName": "Doe",
  "emailId": "john.doe@example.com",
  "department": "IT",
  "salary": 75000
}
```

## 🧪 Testing

### Backend Testing
```bash
cd backend
mvn test
```

### Frontend Testing
```bash
cd frontend
npm test
```

## 📸 Screenshots

_Coming soon..._

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

**Swaroop**
- GitHub: [@swaroop22](https://github.com/swaroop22)
- Email: swrp.vicky@gmail.com

## 🙏 Acknowledgments

- Spring Boot Documentation
- React Documentation
- MySQL Documentation
