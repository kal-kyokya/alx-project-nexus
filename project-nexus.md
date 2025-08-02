# Building a Backend for a Movie Recommendation App - ProDev BE

## Movie Recommendation Backend
### Real-World Application

This project mirrors real-world backend development scenarios where performance, security, and user-centric design are crucial.
By completing this project, I gain experience with:
•	API development and integration.
•	Implementing caching for high-performance systems.
•	Documenting APIs for ease of frontend integration.

### Overview

This case study focuses on developing a robust backend for a movie recommendation application.
The backend provides APIs for retrieving trending and recommended movies, user authentication, and saving user preferences.
It emphasizes performance optimization and comprehensive API documentation.

### Project Goals

The primary objectives of the movie recommendation app backend are:
•	**API Creation**: Develop endpoints for fetching trending and recommended movies.
•	**User Management**: Implement user authentication and the ability to save favourite movies.
•	**Performance Optimization**: Enhance API performance with caching mechanisms.

### Technologies Used

•	**Django**: For backend development.
•	**PostgreSQL**: Relational database for data storage.
•	**Redis**: Caching system for performance optimization.
•	**Swagger**: For API documentation.

### Key Features
#### API for Movie Recommendations

•	Integrate a third-party movie API (e.g., TMDb) to fetch and serve trending and recommended movie data.
•	Implement robust error handling for API calls.

#### User Authentication and Preferences
•	Implement JWT-based user authentication for secure access.
•	Create models to allow users to save and retrieve favourite movies.

#### Performance Optimization
•	Use Redis for caching trending and recommended movie data to reduce API call frequency and improve response time.

#### Comprehensive Documentation
•	Use Swagger to document all API endpoints.
•	Host Swagger documentation at /api/docs for frontend consumption.

### Implementation Process
#### Git Commit Workflow
##### Initial Setup:

•	feat: set up Django project with PostgreSQL
•	feat: integrate TMDb API for movie data

##### Feature Development:
•	feat: implement movie recommendation API
•	feat: add user authentication and favourite movie storage

##### Optimization:
•	perf: add Redis caching for movie data

##### Documentation:

•	feat: integrate Swagger for API documentation
•	docs: update README with API details

### Submission Details
•	Deployment: Host the API and Swagger documentation.

### Evaluation Criteria
#### Functionality

•	APIs retrieve movie data accurately.
•	User authentication and favourite movie storage work seamlessly.

#### Code Quality
•	Code is modular, maintainable, and well-commented.
•	Implements Python best practices and uses Django ORM effectively.

#### Performance
•	Caching with Redis improves API response times.
•	Optimized database queries ensure scalability.

#### Documentation
•	Swagger documentation is detailed and accessible.
•	README includes clear setup instructions.
