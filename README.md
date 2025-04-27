# Airbnb Clone Project

## Overview
This project is a functional clone of Airbnb, built to demonstrate proficiency in modern full-stack development practices. It implements core features of the Airbnb platform while focusing on scalable architecture, security, and collaborative development workflows.

## Learning Objectives
- Master collaborative team workflows using GitHub
- Deepen understanding of backend architecture and database design principles
- Implement advanced security measures for API development
- Gain proficiency in designing and managing CI/CD pipelines
- Strengthen documentation and planning skills for complex software projects
- Develop expertise in integrating Django, MySQL, and GraphQL in a unified ecosystem

## Technology Stack
- **Backend**: Django
- **Database**: MySQL
- **API**: GraphQL
- **Containerization**: Docker
- **CI/CD**: GitHub Actions
- **Version Control**: Git/GitHub

## Requirements
- GitHub account for repository management
- Working knowledge of Markdown syntax
- Experience with Django and MySQL
- Understanding of software development lifecycle practices
- Familiarity with Docker, GitHub Actions, or similar CI/CD platforms

## Getting Started
*Instructions for setup and installation to be added as the project progresses*

## Features
*Feature list to be expanded as development continues*

## Contributors
*List of contributors will be added here*
## Team Roles

- **Backend Engineer**: Responsible for Django application development, API endpoints, and server-side logic
- **Database Administrator**: Manages MySQL database schema, optimizes queries, and ensures data integrity
- **Frontend Developer**: Creates responsive UI components and implements client-side functionality
- **DevOps Engineer**: Handles Docker containerization, CI/CD pipeline configuration, and deployment strategies
- **QA Specialist**: Conducts testing, identifies bugs, and ensures overall application quality
- **Project Manager**: Coordinates team efforts, tracks progress, and manages project timelines
- **Security Specialist**: Implements authentication, authorization, and ensures data protection measures

## Technology Stack
### Technology Stack Details

- **Django**: Python-based web framework powering the backend application logic and MVC architecture
- **MySQL**: Relational database management system for structured data storage and retrieval
- **GraphQL**: Query language for APIs, providing a more efficient alternative to REST
- **Docker**: Platform for developing, shipping, and running applications in containers
- **GitHub Actions**: CI/CD automation tool integrated with the GitHub repository
- **Git/GitHub**: Version control system and platform for collaborative development workflow
## Database Design
### Key Entities
#### Users
- **user_id**: Unique identifier for each user
- **email**: User's email address (used for authentication)
- **name**: User's full name
- **profile_picture**: URL to user's profile image
- **date_joined**: When the user created their account

#### Properties
- **property_id**: Unique identifier for each property
- **host_id**: Reference to the user who owns this property
- **title**: Property listing title
- **location**: Address/geographic coordinates
- **price_per_night**: Base nightly rate
- **description**: Detailed property description

#### Bookings
- **booking_id**: Unique identifier for each booking
- **property_id**: Reference to the booked property
- **guest_id**: Reference to the user making the booking
- **check_in_date**: Start date of stay
- **check_out_date**: End date of stay
- **total_price**: Total cost of the booking

#### Reviews
- **review_id**: Unique identifier for each review
- **booking_id**: Reference to the booking this review is for
- **rating**: Numerical rating (typically 1-5)
- **comment**: Text feedback from the guest
- **date_posted**: When the review was submitted

#### Payments
- **payment_id**: Unique identifier for each payment
- **booking_id**: Reference to the associated booking
- **amount**: Payment amount
- **status**: Payment status (pending, completed, failed)
- **transaction_date**: When the payment was processed

### Entity Relationships

- A User can have multiple Properties (as a host)
- A User can have multiple Bookings (as a guest)
- A Property can have multiple Bookings
- A Booking belongs to exactly one Property and one User (guest)
- A Review belongs to exactly one Booking
- A Payment belongs to exactly one Booking

## License
*License information to be added*