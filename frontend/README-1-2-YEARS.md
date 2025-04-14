# Frontend Assessment (1–2 Years Experience)

## Overview

Welcome to the **1–2 Years** frontend assessment! Your main task is to **replicate a design** on the homepage of this Next.js app. We'll provide a design mockup that you'll need to implement with attention to detail. You'll work on a separate Git branch named after yourself, commit your changes, and open a Pull Request.

## Task Summary

1. **Use Next.js** (version 15 or the current stable release)
2. Implement the design on the main page (`app/page.tsx`)
3. Keep the look and layout **as close as possible** to the provided design mockup
4. Ensure **responsive behavior** for desktop and mobile viewports
5. Complete the task within **1–2 days**

## Design Mockup

(https://www.moola.com/)

The above mockup shows the landing page you need to implement. Pay special attention to:

- Typography and font sizes
- Spacing between elements
- Color scheme
- Responsive behavior
- Button styles and hover states

## Technical Requirements

- Use **Next.js 15** with the App Router
- Implement with **TypeScript**
- Style using **Tailwind CSS** (already configured in the project)
- Ensure the page is **fully responsive**
- Follow accessibility best practices
- Implement basic interactions (hover states, etc.)

## Steps to Complete

### 1. Create & Switch to a New Branch

1. Clone or pull the latest version of this repository.
2. From your local repo folder, run:
   ```bash
   git checkout -b firstname-lastname/frontend
   ```
   Replace `firstname-lastname` with your actual name.
3. Confirm you're on the new branch:
   ```bash
   git branch # You should see your new branch highlighted
   ```

### 2. Implement the Design

1. Open `app/page.tsx` in your code editor.
2. Use Tailwind CSS to style your components.
3. Reference the design mockup for layout, colors, typography, etc.
4. Create additional components under the `components/` directory as needed.
5. Ensure your implementation is responsive and works well on different screen sizes.

### 3. Test Your Work

1. Install dependencies and run the development server:
   ```bash
   npm install
   npm run dev
   ```
2. Open http://localhost:3000 in your browser.
3. Confirm the homepage matches (or closely follows) the design.
4. Test on different viewport sizes to ensure responsiveness.
5. Check for any console errors or warnings.

### 4. Commit & Push

1. Stage and commit your changes:
   ```bash
   git add .
   git commit -m "Implement design on homepage"
   ```
2. Push your branch to the remote repository:
   ```bash
   git push origin firstname-lastname/frontend
   ```

### 5. Open a Pull Request (PR)

1. Go to the repository's page on GitHub (or your Git hosting platform).
2. You should see an option to **"Compare & pull request"** for your new branch, or click **"New pull request."**
3. Select your branch as the source.
4. Give the PR a clear title (e.g., `"Feature: [Your Name] - Frontend UI Implementation"`).
5. In the description, include:
   - How closely you followed the design
   - Any challenges you faced
   - Any decisions or trade-offs you made
   - Browser compatibility notes
6. Submit the PR for review.

## Evaluation Criteria

Your submission will be evaluated based on:

1. **Visual Accuracy**: How closely your implementation matches the design
2. **Code Quality**: Clean, readable, and well-organized code
3. **Responsiveness**: How well the UI adapts to different screen sizes
4. **Attention to Detail**: Colors, spacing, typography, and visual elements
5. **Best Practices**: Semantic HTML, accessibility, and performance considerations

## Time Estimate

This assessment should take approximately 1–2 days to complete. The extended timeline allows you to:

- Pay attention to details in the UI implementation
- Ensure your code is clean and well-structured
- Test thoroughly on different browsers and device sizes
- Refine any animations or interactions

**Good luck, and happy coding!**
