# Issue-Tracker
A modern issue tracking and project management system built with JavaFX, designed to streamline collaboration between project managers and development teams. The application provides a comprehensive solution for tracking issues, managing projects, and facilitating team communication.

## Key Features
- **Role-Based Access Control**: Secure authentication system with distinct interfaces for Administrators, Project Managers, and Developers
- **Project Management**: Create and manage projects with detailed tracking of issues and team assignments
- **Issue Tracking**: Comprehensive bug and issue tracking system with status updates and priority management
- **Team Collaboration**: Built-in commenting system for effective team communication
- **Real-time Updates**: Instant notification system for issue status changes and assignments
- **User-Friendly Interface**: Modern, intuitive GUI built with JavaFX and Scene Builder

## Technical Stack
- **Frontend**: JavaFX 17 with Scene Builder
- **Backend**: Java
- **Database**: MySQL
- **Architecture**: MVC (Model-View-Controller) Design Pattern
- **Build Tool**: Maven

## Getting Started

### Prerequisites
- Java Development Kit (JDK) 17 or higher
- MySQL Server
- Maven
- Scene Builder (for GUI modifications)

### Installation
1. Clone the repository
2. Set up the database using the SQL scripts in the `Database Models` directory
3. Configure database connection in `src/dbUtil/DBConnection.java`
4. Build the project using Maven
5. Run the application using the `GUIStart` class

### Database Configuration
Update the following variables in `src/dbUtil/DBConnection.java`:
```java
url = "your_database_url"
USERNAME = "your_username"
PASSWORD = "your_password"
```

### Running the Application
1. Open the project in your IDE
2. Set the `GUIStart` class as the main class
3. Add the following VM options:
```
--module-path "javafx-sdk-17/lib" --add-modules=javafx.controls,javafx.fxml
```

## Project Structure
```
src/
├── Controller/    # Business logic and event handlers
├── Model/        # Data models and database operations
├── View/         # FXML files and UI components
└── dbUtil/       # Database utilities and connection management
```

## Design Patterns
- **MVC Architecture**: Separation of concerns between data, presentation, and business logic
- **SOLID Principles**: Implementation of Single Responsibility and Open-Closed principles
- **Repository Pattern**: Clean data access layer for database operations

## Common Issues and Solutions
1. **JavaFX Runtime Components Missing**
   - Solution: Add JavaFX SDK to project dependencies
   - Configure VM options as specified above

2. **Database Connection Issues**
   - Verify database credentials
   - Ensure MySQL server is running
   - Check network connectivity

3. **Build Errors**
   - Clean and rebuild the project
   - Update Maven dependencies
   - Verify JDK version compatibility

## Screenshots
[Login Interface]
[Project Dashboard]
[Issue Management]
[Team Collaboration]

## Contributing
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details



