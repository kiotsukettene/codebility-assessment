# Mobile Assessment (5+ Years Experience)

## Overview

Welcome to the **Senior** (5+ years) mobile development assessment!  
This challenge evaluates your ability to build a sophisticated, production-quality **food delivery application** with advanced architecture, performance optimization, offline capabilities, and real-world complex features. You'll demonstrate your mastery of React Native development practices, state management, and technical leadership.

**Branch Requirement**: Please work on a branch named `firstname-lastname/5-years-plus-mobile` (replacing `firstname-lastname` with your own).

## Task Summary

Build a **food delivery application** with the following key features:

1. **Restaurant discovery** screen with filtering and search
2. **Restaurant details** screen with menu categories and items
3. **Cart management** with offline persistence
4. **Checkout flow** with address selection and payment method
5. **Order tracking** screen with simulated status updates
6. **Performance optimizations** for smooth 60fps animations
7. **Offline support** for critical app features
8. **Unit and integration tests** for core functionality
9. **CI configuration** for mobile testing
10. **Documentation** of architecture decisions

## Timeline

- **Duration**: 3-6 days
- This extended timeline allows for a comprehensive implementation
- You may submit earlier if completed, but use the time to ensure quality and proper architecture

## Technical Requirements

### Core Technology Stack

- **React Native**: Expo or bare workflow
- **State Management**: Redux Toolkit or your preferred solution
- **Navigation**: React Navigation with deep linking
- **Storage**: Async Storage or Realm for offline data
- **Networking**: RTK Query, SWR, or custom implementation
- **Testing**: Jest and React Native Testing Library
- **UI Components**: Custom components with animations
- **Typings**: TypeScript with strict mode

### System Architecture

Implement a **modular architecture** with the following components:

1. **Feature-based Organization**

   - Separate modules for restaurants, cart, checkout, and orders
   - Domain-specific hooks, state, and components
   - Shared UI component library

2. **State Management**

   - Centralized store with slices for different domains
   - Middleware for side effects
   - Persistence layer for offline support
   - Optimistic updates for better UX

3. **Navigation**

   - Type-safe navigation setup
   - Deep linking support
   - Navigation state persistence
   - Screen transitions and animations

4. **Data Layer**
   - API client with caching
   - Offline-first data strategy
   - Data synchronization mechanism
   - Mock server for development

### Advanced Features to Implement

1. **Restaurant Discovery**

   - Location-based restaurant filtering
   - Search with debounced input
   - Animated filter transitions
   - Skeleton loading state
   - Pull-to-refresh functionality

2. **Restaurant Details & Menu**

   - Parallax header effect
   - Sticky category navigation
   - Item customization modal
   - Favorites functionality
   - Image lazy loading

3. **Cart Management**

   - Add/remove items with animations
   - Item quantity adjustment
   - Persistent cart storage
   - Offline cart editing
   - Cart summary calculations

4. **Checkout Flow**

   - Multi-step checkout process
   - Address selection with map integration
   - Payment method selection
   - Order summary review
   - Order confirmation with success animation

5. **Order Tracking**

   - Real-time order status updates (simulated)
   - Order history with offline access
   - Delivery ETA display
   - Animated status indicators
   - Order cancellation functionality

6. **Performance Optimizations**
   - Component memoization
   - List virtualization for long scrolling lists
   - Image optimization
   - Transition animations optimization
   - JavaScript thread performance

## Steps to Complete

### 1. Create & Switch to a New Branch

git checkout -b firstname-lastname/5-years-plus-mobile

Replace `firstname-lastname` with your actual name.

### 2. Project Structure & Architecture

Create a modular, scalable project structure:

```
src/
├── api/
│   ├── client.ts
│   ├── endpoints/
│   └── mocks/
├── components/
│   ├── common/
│   └── features/
├── features/
│   ├── restaurants/
│   ├── cart/
│   ├── checkout/
│   └── orders/
├── hooks/
│   ├── common/
│   └── features/
├── navigation/
│   ├── RootNavigator.tsx
│   ├── types.ts
│   └── linking.ts
├── store/
│   ├── index.ts
│   └── slices/
├── theme/
│   ├── colors.ts
│   ├── spacing.ts
│   └── typography.ts
├── utils/
│   ├── storage.ts
│   ├── formatters.ts
│   └── validators.ts
└── App.tsx
```

### 3. Implement Core Functionalities

#### Restaurant Discovery

- Implement restaurant listing with filtering
- Create search functionality with debounce
- Add pull-to-refresh and lazy loading

#### Restaurant Details

- Create restaurant details screen with menu categories
- Implement item details modal
- Add "Add to Cart" functionality

#### Cart Management

- Implement cart state management
- Add persistence for offline usage
- Create cart summary component

#### Checkout Flow

- Build multi-step checkout process
- Implement address selection (simulated)
- Create payment method selection (simulated)

#### Order Tracking

- Create order tracking screen
- Implement simulated status updates
- Build order history feature

### 4. Performance Optimizations

- Optimize list rendering with `FlashList` or similar
- Implement proper memoization for components
- Add skeleton screens for loading states
- Optimize animations for 60fps performance

### 5. Testing

- Write unit tests for core business logic
- Create integration tests for main user flows
- Add snapshot tests for key components

### 6. Documentation

- Document architecture decisions
- Create component documentation
- Add setup instructions

### 7. Commit & Push

git add .
git commit -m "Implement food delivery app with advanced architecture"
git push origin firstname-lastname/5-years-plus-mobile

### 8. Open a Pull Request (PR)

Create a detailed PR with:

- Architecture overview and design decisions
- Screenshots or GIFs of the implementation
- Performance optimization explanations
- Testing strategy
- Future improvements

## Mock API Integration

Use a combination of these approaches for the mock backend:

1. **Local Data**: Include a set of sample restaurant and menu data
2. **JSON Server**: Set up a simple mock server (optional)
3. **MSW (Mock Service Worker)**: For simulating API requests
4. **Simulated Delays**: Add realistic network delays

## Evaluation Criteria

Your submission will be evaluated on:

1. **Architecture**: Clean, maintainable, and scalable code structure
2. **Performance**: Smooth animations, efficient rendering, and loading states
3. **UX/UI**: Intuitive flow, polished animations, and responsive design
4. **Offline Support**: Functioning core features without network connection
5. **Code Quality**: Clean code, proper TypeScript usage, and best practices
6. **Testing**: Comprehensive test coverage and testing strategy
7. **Documentation**: Codebase documentation and architecture explanations

## Bonus Points

- Implementation of accessibility features
- Dark mode support with theme switching
- Analytics integration
- App-wide error boundary implementation
- Advanced animation patterns (shared element transitions)

## Time Estimate

This assessment should take approximately 3-6 days to complete. The extended timeline allows you to:

- Develop a comprehensive, production-quality application
- Implement proper architecture and design patterns
- Create reusable components and utilities
- Add thorough testing coverage
- Optimize performance and user experience
- Document your code and architecture decisions

You're encouraged to make strategic decisions about what to prioritize and implement fully versus what to outline as future work.

**Document any unimplemented features or next steps in your PR.**

We look forward to seeing your senior-level mobile solution!
