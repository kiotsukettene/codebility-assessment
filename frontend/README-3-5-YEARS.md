# Frontend Assessment (3–5 Years Experience)

## Overview

Welcome to the **3–5 Years** frontend assessment!  
This task involves integrating data fetching, dynamic routing, and a bit of React state management. The scope is intended for a mid-level developer who can spend around **2–4 days** on the challenge.

## Task Summary

1. **Use Next.js** (current stable release).
2. Fetch data from a public API and display it in a list page (e.g., `/articles`).
3. Implement a **dynamic route** for item details (e.g., `/articles/[id]`).
4. Include a **like/favorite** feature with basic React state (or local storage).
5. Ensure **basic responsiveness** and a clean UI (no need for pixel-perfect design).
6. Work on a **new branch** named `firstname-lastname/3-5-Years-frontend` before opening a PR.

## Steps to Complete

### 1. Create & Switch to a New Branch

1. Clone or pull the latest version of this repository.
2. From your local repo folder, run:

- git checkout -b `firstname-lastname/3-5-Years-frontend`
  Replace firstname-lastname with your actual name.

3. Confirm you’re on the new branch:

- git branch

# You should see your new branch highlighted

### 2. Data Fetching & Display

1. Choose a public API (e.g., JSONPlaceholder or Fake Store API).

2. Create a new page (e.g., pages/articles/index.tsx) to:

- Fetch a list of items (e.g., articles, products, or posts).

- Display them in a responsive list or grid layout.

- Handle loading and error states gracefully.

### 3. Dynamic Routing

- Implement a dynamic route (e.g., pages/articles/[id].tsx).

- On this page, fetch the details for a single item based on the id.

- Display the item’s details in a clear layout.

### 4. Like/Favorite Feature

1. Allow the user to “like” or “favorite” the item on its detail page.

2. Store the liked state in either:

- React state at the page/component level, or

- Local storage for simple persistence.

3. Indicate on the main list which items are liked/favorited (optional but nice to have).

### 5. Basic UI & Responsiveness

1. Ensure the layout adapts to different screen sizes.

2. Use any styling approach you prefer (CSS modules, Tailwind, etc.).

3. Keep things clean and straightforward (no need for elaborate design).

### 6. Commit & Push

Stage and commit your changes:

- git add .
- git commit -m "Implement data fetch, dynamic routing, and favorite feature"
  Push your branch to the remote repository:

- git push origin `firstname-lastname/3-5-years-frontend`

### 7. Open a Pull Request (PR)

1. Go to the repository on GitHub (or your Git hosting platform).

2. Look for “Compare & pull request” or click “New pull request.”

3. Select your branch (`firstname-lastname/3-5-years-frontend`) as the source.

4. Give the PR a clear title (e.g., "Feature: [Your Name] - 3–5 Years Frontend Challenge").

5. In the description, mention:

- Your approach to fetching data and routing.

- Any challenges or edge cases encountered.

- Any areas you might improve with more time.

6. Submit the PR for review.

### Time Estimate

- Plan for 2–4 days. If you need extra time or skip any part, please note it in your PR.

### Tips

- Keep code readable and well-structured.

- Demonstrate a clear grasp of React hooks and Next.js routing.

- Focus on basic performance (avoid unnecessary re-renders).

- Document any assumptions or simplifications you made.

### Good luck, and happy coding!
