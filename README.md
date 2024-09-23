# **Connect-IT**

## **Project Overview**
The Contact Management System is a web-based application that allows users to manage their contacts efficiently. Users can add new contacts, update existing ones, delete unwanted contacts, and view detailed information for each contact. The project is built using a modern technology stack, including React.js for the frontend, Spring Boot for the backend, and MySQL for the database.

## **Technology Stack**
- **Frontend**: React.js
- **Backend**: Spring Boot (Java)
- **Database**: MySQL
- **Tools**: Maven, Spring Data JPA, RESTful APIs
- **Version Control**: Git and GitHub

## **Features**
- **Add Contact**: Create a new contact with details like name, email, phone number, address ,status, profile picture.
- **View Contacts**: List all contacts with pagination support.
- **Update Contact**: Modify existing contact details.
- **Delete Contact**: Remove a contact from the system.

## **Screenshot**
 ![2](https://github.com/user-attachments/assets/2c745e10-3f90-41ae-9d5a-4e3dd3b7d40b)

![1](https://github.com/user-attachments/assets/8a1b1400-15e8-49fd-8bbe-fa981b7c69df)

## **Installation**
### **Prerequisites**
Before you begin, ensure you have the following installed on your system:
- **Java 8+** (for backend)
- **Node.js** and **npm** (for frontend)
- **MySQL** (for the database)
- **Maven** (for backend dependency management)
- **Git** (for version control)

### **Backend Setup**
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/amitkr-15/Connect-IT
   cd Connect IT-Sever
   ```
2. **Configure the MySQL Database:**
   - Create a database named `testdatabase` in MySQL.
   - Update the `src/main/resources/application.properties` file with your MySQL credentials:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/testdatabase
     spring.datasource.username=your-username
     spring.datasource.password=your-password
     spring.jpa.hibernate.ddl-auto=update
     ```
3. **Build and Run the Backend:**
   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

### **Frontend Setup**
1. **Navigate to the Frontend Directory:**
   ```bash
   cd ../Connect_it-client
   ```
2. **Install Dependencies:**
   ```bash
   npm install
   ```
3. **Run the React App:**
   ```bash
   npm start
   ```
4. The application will be accessible at `http://localhost:3000`.

## **API Endpoints**

### **Contact Management**
- **Get All Contacts**
  - `GET /api/contacts`
- **Get Contact by ID**
  - `GET /api/contacts/{id}`
- **Add New Contact**
  - `POST /api/contacts`
- **Update Contact**
  - `PUT /api/contacts/{id}`
- **Delete Contact**
  - `DELETE /api/contacts/{id}`
