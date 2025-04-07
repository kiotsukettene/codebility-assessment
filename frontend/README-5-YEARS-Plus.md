# Frontend Assessment (5+ Years Experience)

## Overview

Welcome to the **Senior** (5+ years) frontend assessment!  
This challenge is designed to test your **architecture decisions**, **code quality**, and **advanced usage** of React/Next.js. You'll integrate **multiple data sources**, focus on performance, and demonstrate best practices with Next.js 15's App Router and React Server Components.

**Branch Requirement**: Please work on a branch named `firstname-lastname/5-years-plus` (replacing `firstname-lastname` with your own).

## Task Summary

1. **Build a dashboard application** with multiple sections (overview, analytics, user management, etc.)
2. **Fetch data from these specific APIs**:
   - [OpenWeatherMap API](https://openweathermap.org/api) - For weather data visualization
   - [Finnhub Stock API](https://finnhub.io/) - For financial market data
   - (Free API keys are available for both services with reasonable usage limits)
3. **Implement modern data fetching**:
   - Server Components for initial data loads
   - Client Components with React Query/SWR for interactive elements
   - Proper loading and error states using Next.js 15 features
4. **Next.js 15 Architecture**:
   - Leverage the App Router
   - Use React Server Components appropriately
   - Implement parallel data fetching where beneficial
   - Apply proper client/server component boundaries
5. **Performance Optimization**:
   - Implement Suspense boundaries intelligently
   - Use dynamic imports for code splitting
   - Create a responsive design with minimal layout shifts
6. **Testing**: Add meaningful tests using React Testing Library and Jest or Vitest
7. **Styling**: Create a clean, well-structured dashboard following modern design principles
8. Allow **3–6 days** for this challenge (though the depth is up to you)

## Steps to Complete

### 1. Create & Switch to a New Branch

1. Pull or clone the latest version of this repository.
2. From your local repo, create a new branch:

   git checkout -b firstname-lastname/5-years-plus

   Replace `firstname-lastname` with your actual name.

3. Confirm your new branch:

   git branch # Your new branch should be highlighted

### 2. Dashboard & Data Architecture

1. Set up a dashboard using Next.js 15 App Router (app/ directory structure)
2. Create multiple sections with the following recommended structure:

   app/
   ├── dashboard/
   │ ├── page.tsx # Main dashboard page (Server Component)
   │ ├── layout.tsx # Dashboard layout with navigation
   │ ├── loading.tsx # Loading state
   │ ├── error.tsx # Error handling
   │ ├── weather/
   │ │ └── page.tsx # Weather data section
   │ └── finance/
   │ └── page.tsx # Financial data section
   ├── api/ # API routes if needed
   └── components/
   ├── server/ # Server Components
   └── client/ # Client Components

3. API Integration:

   - Weather Section: Fetch and display current weather and forecasts from OpenWeatherMap
   - Finance Section: Show stock data and price charts from Finnhub
   - Implement proper error handling, loading states, and data refresh strategies

4. Server/Client Components:
   - Use Server Components for initial data fetching and SEO
   - Use Client Components for interactive elements like:
     - Weather location selector
     - Stock symbol search
     - Data refresh controls
     - Interactive charts

### 3. Performance Considerations

1. Implement **streaming** with Suspense for progressive loading of dashboard sections
2. Use Next.js 15's recommended caching strategies:
   - Leverage the built-in fetch cache for Server Components
   - Use React Query or SWR for client-side data that needs refreshing
3. Apply dynamic imports with `next/dynamic` for code splitting
4. Optimize and lazy-load any third-party visualization libraries

### 4. Testing

1. Write tests focusing on:
   - Component rendering and interactions
   - Data fetching logic
   - Error state handling
2. Recommended tools:
   - React Testing Library
   - Jest or Vitest
   - MSW (Mock Service Worker) for API mocking

### 5. Commit & Push

1. Stage and commit your changes:

   git add .
   git commit -m "Implement advanced dashboard with weather and financial APIs"

2. Push your branch to the remote repository:

   git push origin firstname-lastname/5-years-plus

### 6. Open a Pull Request (PR)

1. Go to the repository in your Git hosting platform.
2. Create a new pull request with your branch as the source.
3. Use a clear title (e.g., "Feature: [Your Name] - 5+ Years Frontend Dashboard").
4. In the description, highlight:
   - Your architecture decisions regarding Server vs Client Components
   - Caching and data fetching strategies
   - Performance optimizations implemented
   - Testing approach
   - Any challenges or areas for future improvement

## Evaluation Criteria

Your solution will be evaluated based on:

1. **Architecture**: Proper use of Next.js 15 features and patterns
2. **Component Design**: Clear separation of concerns and reusable components
3. **Data Handling**: Efficient data fetching and state management
4. **Performance**: Smart implementation of React Server Components and client optimizations
5. **Code Quality**: Clean, readable, and well-documented code
6. **Testing**: Meaningful tests that verify key functionality

## Time Estimate

This test is designed to take 3–6 days for a minimal implementation. Feel free to detail any unimplemented features or next steps in your PR if you run out of time.

## Tips

- Begin with scaffolding the app structure and implementing the basic data fetching
- Use placeholder UIs while working on the architecture
- If API rate limits become an issue, consider implementing a simple caching layer or mock data
- Focus on demonstrating your understanding of modern Next.js patterns rather than visual polish

### We look forward to reviewing your solution!
