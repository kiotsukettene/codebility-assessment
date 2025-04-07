# Backend Assessment (5+ Years Experience)

## Overview

Welcome to the **Senior** backend assessment!  
This challenge evaluates your ability to design and implement a **scalable, production-ready** backend architecture. You'll demonstrate advanced patterns, performance optimization, security best practices, and DevOps considerations.

**Branch**: `firstname-lastname/5-years-plus` (replace `firstname-lastname` with your own name).

## Task Summary

Build a **robust e-commerce backend API** that showcases:

1. **Domain-Driven Design** principles with clear bounded contexts
2. **Microservices communication** patterns (at least 2 services)
3. **Advanced authentication** with role-based access control
4. **Database performance optimization** techniques
5. **Background job processing** for async operations
6. **Comprehensive testing** strategy
7. **Containerization** with Docker and Docker Compose
8. **API documentation** with OpenAPI/Swagger
9. **Observability** setup (logging, monitoring)
10. **CI pipeline** configuration

## Technical Requirements

### Core Technology Stack

- **Node.js**: v20+ LTS
- **TypeScript**: Strong typing throughout
- **Framework**: Express.js or NestJS
- **Database**: PostgreSQL + Redis
- **ORM**: Prisma or TypeORM
- **Authentication**: JWT with refresh tokens
- **Message Queue**: Redis or RabbitMQ
- **Containerization**: Docker + Docker Compose
- **Testing**: Jest + Supertest
- **Documentation**: OpenAPI/Swagger
- **CI**: GitHub Actions workflow

### System Architecture

Implement a **microservices architecture** with the following components:

1. **API Gateway Service**

   - Route requests to appropriate services
   - Handle authentication and authorization
   - Rate limiting and basic caching
   - Request validation

2. **User Service**

   - User registration and authentication
   - Profile management
   - Role-based permissions
   - Password reset flow

3. **Product Service**

   - Product CRUD operations
   - Inventory management
   - Search and filtering
   - Category management

4. **Order Service**
   - Order creation and management
   - Integration with external payment API
   - Async order processing with queues
   - Email notifications (simulated)

### Advanced Features to Implement

1. **Authentication & Security**

   - JWT with refresh token rotation
   - Role-based access control (RBAC)
   - API rate limiting
   - Input sanitization and validation
   - Security headers

2. **Database & Performance**

   - Database migrations
   - Indexing strategy
   - Query optimization
   - Connection pooling
   - Data pagination

3. **Background Processing**

   - Job queue for async operations
   - Retry mechanisms
   - Dead letter queues
   - Scheduled jobs

4. **Error Handling & Reliability**

   - Centralized error handling
   - Circuit breakers for external services
   - Graceful shutdowns
   - Request correlation IDs

5. **Observability**
   - Structured logging
   - Request tracing
   - Health check endpoints
   - Prometheus metrics (optional)

## Steps to Complete

### 1. Create & Switch to a New Branch

git checkout -b `firstname-lastname/5-years-plus`

### 2. Project Setup & Architecture

Create a monorepo structure with the following organization:

```
backend/
├── services/
│   ├── api-gateway/
│   ├── user-service/
│   ├── product-service/
│   └── order-service/
├── shared/
│   ├── types/
│   ├── utils/
│   └── config/
├── docker/
│   ├── docker-compose.yml
│   ├── docker-compose.dev.yml
│   └── Dockerfiles/
├── docs/
│   ├── architecture.md
│   └── api/
├── .github/
│   └── workflows/
└── README.md
```

Each service should have its own:

- Package.json and dependencies
- Database migrations (if applicable)
- Tests directory
- OpenAPI documentation

### 3. Implementation Requirements

#### API Gateway Service:

- Route configuration for all microservices
- Authentication middleware
- Rate limiting implementation
- Request validation and sanitization
- Logging and tracing setup

#### User Service:

- Secure user registration and authentication
- JWT generation with refresh token rotation
- Password hashing with bcrypt
- Role and permission management
- Profile management endpoints

#### Product Service:

- Complete CRUD for products
- Category management
- Search and filtering capabilities
- Inventory tracking
- Image URL management (no file uploads required)

#### Order Service:

- Order creation and management
- Integration with mock payment service
- Background processing using queue
- Email notification service (simulated)
- Order status transitions

### 4. Data Storage and Communication

- Use PostgreSQL for persistent data
- Implement Redis for caching and session management
- Set up a message queue for service communication
- Implement proper database indexes and query optimization

### 5. DevOps & Infrastructure

- Create Dockerfiles for each service
- Configure Docker Compose for local development
- Implement GitHub Actions for CI pipeline
- Include database migrations in deployment process

### 6. Testing Strategy

- Unit tests for business logic
- Integration tests for API endpoints
- E2E tests for critical user flows
- Performance tests (optional)

### 7. Documentation

- OpenAPI/Swagger documentation for all endpoints
- Architecture documentation explaining design decisions
- Setup and installation instructions

### 8. Commit & Push

```bash
git add .
git commit -m "Implement microservices architecture with advanced patterns"
git push origin firstname-lastname/5-years-plus
```

### 9. Open a Pull Request (PR)

Create a detailed PR with:

- Architecture overview and design decisions
- Setup instructions
- Testing approach
- Performance considerations
- Security measures implemented
- Future improvements

## External Service Integration

Integrate with at least **two** of these external services:

1. **Payment Processing**: Stripe API (test mode)
2. **Email Service**: Nodemailer with Ethereal (fake SMTP service)
3. **Geocoding**: OpenCage or Google Maps Geocoding API
4. **Currency Conversion**: Exchange Rates API

## Evaluation Criteria

Your submission will be evaluated on:

1. **System Design**: Architecture decisions, service boundaries, and scalability considerations
2. **Code Quality**: Clean code, design patterns, and best practices
3. **Performance**: Database optimization, caching strategies, and async processing
4. **Security**: Authentication, authorization, and general security practices
5. **DevOps**: Docker setup, CI configuration, and deployment strategy
6. **Testing**: Comprehensive test coverage and testing strategy
7. **Documentation**: API docs, architecture explanations, and setup instructions

## Bonus Points

- Implementation of event sourcing patterns
- Command Query Responsibility Segregation (CQRS)
- Feature flags or A/B testing capability
- Advanced database features (e.g., PostGIS, JSONB querying)
- Chaos testing or resilience patterns

## Time Estimate

This assessment is designed to take 3–6 hours for a minimal implementation, focusing on architecture rather than complete feature implementation. You're encouraged to make strategic decisions about what to prioritize and implement fully versus what to outline as future work.

**Document any unimplemented features or next steps in your PR.**

We look forward to seeing your senior-level backend solution!
