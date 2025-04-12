# Backend Assessment (3–5 Years Experience)

## Overview

Welcome to the **3–5 Years** backend assessment!  
This challenge involves building a more robust Express.js API with TypeScript, proper architecture, database integration, authentication, and external API integration. We aim to see how you structure a mid-complexity application in **2–4 days**.

## Task Summary

1. **Create a new branch**: `firstname-lastname/3-5-years-backend`
2. Build an **Express.js + TypeScript** application with:
   - **Clean architecture** (services, controllers, repositories)
   - **Database integration** with Prisma ORM
   - **JWT authentication** with role-based access control
   - **External API integration** (OpenWeatherMap or other public API)
   - **Input validation** using Zod or similar
   - **Comprehensive error handling**
   - **Unit and integration tests**

## Technical Requirements

### Features to Implement

1. **User Management**:

   - Registration (`POST /api/auth/register`)
   - Login (`POST /api/auth/login`)
   - Get user profile (`GET /api/users/me`)

2. **Products API**:

   - Create product (admin only) (`POST /api/products`)
   - List all products (`GET /api/products`)
   - Get product by ID (`GET /api/products/:id`)
   - Update product (admin only) (`PUT /api/products/:id`)
   - Delete product (admin only) (`DELETE /api/products/:id`)

3. **Weather Integration**:

   - Get weather for a location (`GET /api/weather?city=CityName`)
   - This endpoint should fetch data from OpenWeatherMap API

4. **Technical Requirements**:
   - Implement JWT authentication
   - Role-based access control (user vs admin)
   - Request validation using Zod schemas
   - Proper error handling with custom error classes
   - Prisma ORM for database operations
   - Unit and integration tests

## Steps to Complete

### 1. Create & Switch to a New Branch

git checkout -b firstname-lastname/3-5-years-backend

Replace `firstname-lastname` with your actual name.

### 2. Implementation Requirements

1. **Authentication**:

   - Implement JWT-based authentication
   - Create middleware to protect routes
   - Implement role-based authorization (admin vs user)

2. **Database Integration**:

   - Use Prisma ORM for database operations
   - Implement repository pattern for data access
   - Handle database errors gracefully

3. **External API Integration**:

   - Weather API integration (OpenWeatherMap or similar)
   - Proper error handling for API failures
   - Response caching if time permits

4. **Input Validation**:

   - Use Zod to validate request bodies
   - Create middleware for validation
   - Return descriptive validation errors

5. **Error Handling**:

   - Create custom error classes
   - Implement global error handling middleware
   - Return consistent error responses

6. **Testing**:
   - Write unit tests for services
   - Write integration tests for API endpoints
   - Use in-memory database for tests if possible

### 5. Testing

1. Set up Jest for testing:

   npx ts-jest config:init

2. Write tests for key functionality:
   - Authentication flow
   - Product CRUD operations
   - External API integration

### 6. Commit & Push

git add .
git commit -m "Implement Express API with authentication, database, and weather integration"
git push origin firstname-lastname/3-5-years-backend

### 7. Open a Pull Request (PR)

1. Go to the repository on GitHub
2. Open a new Pull Request with your branch as the source
3. Give it a descriptive title
4. In the description, include:
   - Overview of your implementation
   - Architecture decisions
   - How to run the application locally
   - How to run tests
   - Any challenges faced or tradeoffs made

## Evaluation Criteria

Your submission will be evaluated based on:

1. **Architecture**: Clean and maintainable code structure
2. **Security**: Proper authentication and authorization
3. **Database**: Efficient use of Prisma and proper data modeling
4. **Error Handling**: Comprehensive error handling and validation
5. **Testing**: Quality and coverage of tests
6. **Documentation**: Clear code documentation and PR description

## Time Estimate

This assessment should take approximately 2–4 days to complete. If you're unable to complete all features, prioritize quality over quantity and document what's missing.

**Good luck, and happy coding!**
