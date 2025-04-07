# Backend Assessment (1–2 Years Experience)

## Overview

Welcome to the **1–2 Years** backend assessment!  
Your goal is to create a **basic Node.js + Express** RESTful API with data validation and proper error handling. This assessment is designed to be completed in **1–2 hours** to demonstrate your fundamental backend development skills.

## Task Summary

1. **Create a new branch**: `firstname-lastname/1-2-years-backend`
2. Set up a modern **Node.js + Express** application with TypeScript
3. Implement **CRUD endpoints** for a "Todo" resource
4. Use **input validation** for all endpoints
5. Implement **proper error handling** with status codes
6. Store data **in-memory** (no database setup required)
7. Write a **simple test** for at least one endpoint

### Features to Implement

1. **Todo API with the following endpoints**:

   - `GET /api/todos` - List all todos
   - `GET /api/todos/:id` - Get a single todo
   - `POST /api/todos` - Create a new todo
   - `PUT /api/todos/:id` - Update a todo
   - `DELETE /api/todos/:id` - Delete a todo

2. **Data Structure**:

   ```typescript
   interface Todo {
     id: string;
     title: string;
     completed: boolean;
     createdAt: Date;
     updatedAt: Date;
   }
   ```

3. **Validation Requirements**:
   - Todo title must be between 3 and 100 characters
   - IDs should be validated as UUIDs
   - Return appropriate 400 errors for invalid input

## Steps to Complete

### 1. Create & Switch to a New Branch

git checkout -b `firstname-lastname/1-2-years-backend`

Replace `firstname-lastname` with your actual name.

### 2. Implement the API

1. **Create the Todo API**:

   - Implement CRUD operations for todos
   - Use UUIDs for todo IDs
   - Include validation for inputs
   - Return appropriate status codes

2. **Basic Error Handling**:

   - Create middleware for handling errors
   - Return appropriate status codes and error messages
   - Ensure all error responses follow a consistent format

3. **Example Implementation**:

   ```typescript
   // src/index.ts
   import express from "express";
   import cors from "cors";
   import todoRoutes from "./routes/todos";
   import errorHandler from "./middleware/error-handler";

   const app = express();
   const PORT = process.env.PORT || 4000;

   app.use(cors());
   app.use(express.json());

   // Routes
   app.use("/api/todos", todoRoutes);

   // Health check
   app.get("/health", (req, res) => {
     res.status(200).json({ status: "ok" });
   });

   // Error handler
   app.use(errorHandler);

   app.listen(PORT, () => {
     console.log(`Server running on http://localhost:${PORT}`);
   });
   ```

### 5. Testing

1. Write at least one simple test for the Todo API
2. Test the GET and POST endpoints

### 6. Commit & Push

```bash
git add .
git commit -m "Implement Todo API with validation and error handling"
git push origin firstname-lastname/1-2-years-backend
```

### 7. Open a Pull Request (PR)

1. Go to the repository on GitHub
2. Open a new Pull Request with your branch
3. Give it a descriptive title
4. In the description, include:
   - Overview of your implementation
   - How to run the API locally
   - Any additional features you implemented

## Evaluation Criteria

Your submission will be evaluated based on:

1. **Code Quality**: Clean, readable code with proper error handling
2. **API Design**: Proper use of HTTP methods and status codes
3. **Validation**: Proper input validation and error responses
4. **Organization**: Logical project structure and file organization
5. **Testing**: Basic test coverage of at least one endpoint

## Time Estimate

This assessment should take approximately 1–2 hours to complete.

**Good luck, and happy coding!**
