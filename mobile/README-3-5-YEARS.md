# Mobile Assessment (3-5 Years Experience)

## Overview

Welcome to the **3-5 Years** mobile development assessment!  
This challenge requires you to build a **functional e-commerce product screen** with API integration, state management, and proper component architecture. You'll demonstrate your skills with React Native, data fetching, and creating a polished user experience.

**Branch Requirement**: Please work on a branch named `firstname-lastname/3-5-years-mobile` (replacing `firstname-lastname` with your own).

## Task Summary

1. Create a **product details screen** with the following sections:
   - Product image gallery/carousel
   - Product information (title, price, rating)
   - Product description
   - Size/variant selector
   - Add to cart functionality
   - Related products section
2. Integrate with the **Fake Store API** to fetch real product data
3. Implement **state management** using your preferred approach
4. Create **reusable components** with proper organization
5. Add **animations and transitions** for a polished UX
6. Include **error handling** and loading states
7. Implement **unit tests** for key components
8. Allow **2-4 days** for this challenge

## Timeline

- **Duration**: 2-4 days
- You're encouraged to utilize the full timeline to ensure quality and completeness
- Early submissions are welcome if you complete the assessment sooner

## Technical Requirements

### Environment

- **React Native**: Use the existing Expo project structure
- **API**: [Fake Store API](https://fakestoreapi.com/) for product data
- **State Management**: Context API, Redux, or your preferred solution
- **Navigation**: React Navigation
- **Testing**: Jest and React Native Testing Library

### Features to Implement

1. **Product Details Screen**:

   - Fetch and display product details from the API
   - Create an image carousel for product images
   - Display product information (title, description, price, rating)
   - Implement a size/variant selector when applicable
   - Add "Add to Cart" button with animation feedback

2. **Related Products**:

   - Fetch products from the same category
   - Display in a horizontal scrollable list
   - Navigate to the selected product when tapped

3. **State Management**:

   - Implement cart functionality (add items, view cart count)
   - Persist cart data (React Context or Redux)
   - Handle loading and error states

4. **UI/UX Enhancements**:
   - Add appealing animations (react-native-reanimated or similar)
   - Implement proper loading states
   - Create error handling UI
   - Ensure responsive layout across device sizes

## Steps to Complete

### 1. Create & Switch to a New Branch

git checkout -b firstname-lastname/3-5-years-mobile

Replace `firstname-lastname` with your actual name.

### 2. Project Structure

Organize your code with a clean component architecture:

```
components/
├── product/
│   ├── ProductGallery.tsx
│   ├── ProductInfo.tsx
│   ├── VariantSelector.tsx
│   └── RelatedProducts.tsx
├── common/
│   ├── Button.tsx
│   ├── Loading.tsx
│   └── ErrorState.tsx
hooks/
├── useProductDetails.ts
├── useRelatedProducts.ts
└── useCart.ts
contexts/
└── CartContext.tsx
screens/
└── ProductScreen.tsx
tests/
└── components/
    └── product/
        └── ProductInfo.test.tsx
```

### 3. API Integration

1. Fetch product data from the Fake Store API:

   ```typescript
   // Example API endpoints
   const getProduct = async (id: number) => {
     const response = await fetch(`https://fakestoreapi.com/products/${id}`);
     return response.json();
   };

   const getRelatedProducts = async (category: string) => {
     const response = await fetch(
       `https://fakestoreapi.com/products/category/${category}`
     );
     return response.json();
   };
   ```

2. Implement loading and error handling for API requests

### 4. State Management

1. Create a cart context or Redux store
2. Implement add to cart functionality
3. Store cart state persistently

### 5. UI/UX Implementation

1. Create a visually appealing product details screen
2. Implement the image carousel with smooth transitions
3. Add animations for user interactions
4. Ensure responsive layout across different device sizes

### 6. Testing

1. Write unit tests for key components
2. Test the add to cart functionality
3. Test API integration with mocked responses

### 7. Commit & Push

git add .
git commit -m "Implement product details screen with API integration"
git push origin firstname-lastname/3-5-years-mobile

### 8. Open a Pull Request (PR)

1. Go to the repository on GitHub
2. Create a new Pull Request with your branch
3. Use a descriptive title
4. In the description, include:
   - Screenshots/GIFs of your implementation
   - Architecture decisions and state management approach
   - Any challenges faced and how you solved them
   - Testing approach

## Evaluation Criteria

Your submission will be evaluated based on:

1. **Functionality**: Working product screen with all required features
2. **Code Quality**: Clean, readable, and well-structured code
3. **Component Architecture**: Proper organization and reusable components
4. **State Management**: Effective state management approach
5. **UI/UX**: Visual appeal, animations, and responsiveness
6. **API Integration**: Proper data fetching, loading states, and error handling
7. **Testing**: Quality and coverage of tests

## Time Estimate

This assessment should take approximately 2-4 days to complete. The extended timeline allows you to:

- Build a more complete and polished implementation
- Create reusable components with proper documentation
- Implement more comprehensive state management
- Add thorough test coverage
- Polish animations and user interactions

If you're unable to complete all features, prioritize quality over quantity and document what's missing.

**Good luck, and happy coding!**
