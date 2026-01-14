# MarketPlace Application

A full-stack marketplace application built with Spring Boot, PostgreSQL, Angular, and JWT authentication. This project demonstrates modern web development practices with secure authentication, RESTful APIs, and a responsive frontend.

## 🚀 Features

- **User Authentication & Authorization**
  - User registration and login
  - JWT-based secure access and refresh token handling
  - Role-based access control

- **Product Management**
  - Product listing and searching
  - Product creation and management
  - Image upload support

- **Buying & Selling**
  - Complete buying and selling functionality
  - User profiles with transaction history
  - Product search and filtering

## 🛠️ Tech Stack

### Backend
- **Spring Boot** - Java framework for building REST APIs
- **PostgreSQL** - Relational database
- **Spring Security** - Security framework
- **JWT** - JSON Web Tokens for authentication
- **Maven** - Dependency management

### Frontend
- **Angular** - Modern web framework
- **TypeScript** - Type-safe JavaScript
- **Tailwind CSS** - Utility-first CSS framework

## 📋 Prerequisites

Make sure you have the following tools installed before setting up the application:

- **Java Development Kit (JDK)** 11 or higher
- **Apache Maven** 3.6+
- **PostgreSQL** 12+
- **Node.js** 16+ and **npm** 8+
- **Angular CLI** (install with `npm install -g @angular/cli`)

## 🔧 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/declared-as-ala/marketplace-_spring_Angular.git
cd MarketPlace
```

### 2. Database Configuration

1. Create a new PostgreSQL database:
   ```sql
   CREATE DATABASE marketplace;
   ```

2. Configure database connection in `src/main/resources/application.yaml`:
   ```yaml
   spring:
     datasource:
       url: jdbc:postgresql://localhost:5432/marketplace
       username: postgres
       password: postgres
   ```
   
   > **Note:** Update the username and password according to your PostgreSQL configuration.

3. Spring Boot will automatically create the necessary tables on startup.

### 3. Backend Setup

1. Navigate to the project root directory
2. Build and run the Spring Boot application:
   ```bash
   mvn spring-boot:run
   ```
   
   The backend API will be available at `http://localhost:8080`

### 4. Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the Angular development server:
   ```bash
   ng serve
   ```
   
   The frontend application will be available at `http://localhost:4200`

## 🎯 Usage

1. **Access the Application**
   - Open your browser and navigate to `http://localhost:4200`

2. **Register a New Account**
   - Click on "Register" to create a new user account
   - Fill in your details and submit

3. **Login**
   - Use your credentials to log in to the application

4. **Start Trading**
   - Browse products on the marketplace
   - Create listings for items you want to sell
   - Search for products you're interested in buying
   - Manage your profile and view your transaction history

## 📁 Project Structure

```
MarketPlace/
├── frontend/                 # Angular frontend application
│   ├── src/
│   │   ├── app/
│   │   │   ├── _guards/     # Route guards
│   │   │   ├── _modules/    # Type definitions
│   │   │   ├── _services/   # API services
│   │   │   └── ...          # Components
│   │   └── assets/          # Static assets
│   └── package.json
├── src/
│   └── main/
│       ├── java/            # Spring Boot backend
│       │   └── com/market/marketplace/
│       │       ├── controllers/    # REST controllers
│       │       ├── services/       # Business logic
│       │       ├── repositories/   # Data access layer
│       │       ├── models/         # Entity models
│       │       ├── dto/            # Data transfer objects
│       │       └── security/       # Security configuration
│       └── resources/
│           └── application.yaml   # Application configuration
└── pom.xml                   # Maven dependencies
```

## 🔐 Security Features

- JWT token-based authentication
- Refresh token mechanism for secure session management
- Password encryption using BCrypt
- CORS configuration for cross-origin requests
- Spring Security integration

## 📝 API Endpoints

The application provides RESTful APIs for:
- Authentication (register, login, refresh token)
- Product listings (create, read, update, delete)
- User profiles (view, update)
- Search functionality

## 🐛 Known Issues & Future Improvements

As noted in the original project, there are areas for improvement:
- Handling duplicate API calls and implementing caching
- Image compression and decompression optimization
- Better API endpoint organization
- Enhanced error handling
- Unit and integration tests

## 📄 License

This project is licensed under the [MIT License](./LICENSE).

## 👨‍💻 About the Author

**Ala Missaoui**

- 📧 Email: [alamissaoui.dev@gmail.com](mailto:alamissaoui.dev@gmail.com)
- 🔗 GitHub: [@declared-as-ala](https://github.com/declared-as-ala)

This project was forked and enhanced to demonstrate full-stack development skills with Spring Boot and Angular, focusing on JWT authentication and Spring Security implementation.

## 🙏 Acknowledgments

- Original project by [confusedGustas](https://github.com/confusedGustas/MarketPlace)
- Built with Spring Boot, Angular, and PostgreSQL

---

**Note:** This project was created for learning purposes, particularly focusing on JWT authentication and Spring Security. While there are areas that could be improved, the core functionality demonstrates a solid understanding of modern web development practices.
