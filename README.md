# AirBnB Clone Project
## Project Overview
This is a simulation of the robust booking platform, Airbnb. The goal of this clone is real-world functionality and scalability with application security. The backend development will use Django, PostgreSQL, GraphQL, Docker and GitHub Actions for CI/CD 

## Project Goals
- Reproduce core functionality for an MVP
- Master agile team  collaboration in fullstack teams
- Implement security for RESTful amd GraphQL APIs
- Enrich understanding of complex software architectures and database esign
- Design and manage CI/CD pipelines for deployment

## Team Roles
- **Backend Engineer**: creates the API, implements algorithms, business logic and database schemas  using Django and GraphQL
- **QA Engineer**: ensures the application performs according to requirements by running tests on functionality, usability, security and performance
- **DevOps engineer**: Sets up and maintains environments using Docker.Builds and maintains CI/CD pipelines for code releases, faster delivery and maintaining application stability
- **Database Administrator**:  Manages the PostgreSQL database design, indexing and optimization



## Technology Stack
- **Django:** web framework for building RESTful APIs
- **PostgreSQL:** a relational database for managing user and property data
- **GraphQL:** query language useful for large,complex and interrelated data
- **Celery:** for handling asynchronous tasks
-** Redis:** a in-memory store for caching and session management
- **Docker:** containerization tool for creating dev environments
-**Github Actions:** CI/CD tool for testing and deploying

## Database Design
- **Users:** ``{ id(pk), name, email, password, profile picture, role}`` 
    *A user can have multiple bookings, properties, reviews and payments*

- **Properties:** ``{id(pk), owner_id(fk), name, price_per_ni total_rooms, address, status}`` 
    *A property can have multiple bookings, reviews and payments*

- **Bookings:**: ``{id(pk), user_id(fk), property_id(fk), payment, start_date, end_date,status}``
    *A booking can have a single user, property and payment*

- **Reviews**: ``{id(pk), property_id(fk), user_id(fk), comment,}`` 
    *A review can have one user and one property*

- **Payments**: ``{id(pk), user_id(fk), property_id(fk), booking, payment_date, amount, status}`` 
    *A payment has a single user, property and booking*

## Feature Breakdown
- **Property Management**: Owners can Create, Update, Read and Delete Property Listings
- **Booking Management**: Guests can Create, Retrieve, Update and Cancel bookings
- **User Authentication**: Guests can Create, authenticate, Delete, Update user profiles
- **Review System**: Guests can Create, Post, Update and Delete reviews
- **Payment Processing**: Guests can process payment with a 3rd-party service

## API Security
- Authentication
- Authorization
- Rate limiting
- Data Encryption
- Input Validation
- Data Monitoring

These security measures  guard against unauthorized access to an application,  unauthorized data access during application use, DDoS attacks, injection attacks, access to sensitive data, and  undetected attacks.

## CI/CD Pipeline
CI/CD pipelines are automated workflows for building, testing and deploying code changes to the desired environment. This helps to reduce human error and increase code quality while helping teams increase collaboration and release new updates faster

### Common CI/CD tools
- Git/Github: for version control
- GitHub Actions: for CI/CD orchestration
- Docker: for consistent development, test and deployment environments
- Kubernetes: for container orchestration and deployment

## Contributors
- Stephanie Olulesho 