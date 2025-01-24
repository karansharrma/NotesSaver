## Installation

### Step 1: Create a Vite project

1. Install Vite globally (if not already installed):

   ```bash
   npm create vite@latest
   ```

2. When prompted, choose the following:
   - Project name: `NotesSaver`
   - Framework: `React`
   - Variant: `JavaScript` or `TypeScript` as per your preference.

3. Navigate into the project directory:

   ```bash
   cd NotesSaver
   ```

### Step 2: Install Tailwind CSS

1. Install Tailwind CSS and its dependencies:

   npm install -D tailwindcss postcss autoprefixer
  
2. Initialize Tailwind configuration:

   npx tailwindcss init
 
   This will create a `tailwind.config.js` file in your project.

3. Update the `tailwind.config.js` file with the following content to specify which files Tailwind should scan:

   ```js
   /** @type {import('tailwindcss').Config} */
   export default {
     content: [
       './index.html',
       './src/**/*.{js,ts,jsx,tsx}',
     ],
     theme: {
       extend: {},
     },
     plugins: [],
   }
   ```

4. Add the following lines to your `src/index.css` (or `src/main.css` if you’re using that):

   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

### Step 3: Install Required Packages

Install the project dependencies:

npm install


### Step 4: Run the Project
npm run dev

## Scripts

- **`npm run dev`**: Starts the Vite development server with HMR.
- **`npm run build`**: Builds the project for production.
- **`npm run preview`**: Serves the production build for preview.
- **`npm run lint`**: Lints your code using ESLint.

---

## Packages Used

Here is a list of all the important packages used in this project:

### Dependencies
- **@reduxjs/toolkit**: A powerful library for managing application state with Redux.
- **lucide-react**: Icon set for React that provides various UI icons.
- **react**: The core React library for building user interfaces.
- **react-dom**: DOM bindings for React.
- **react-hot-toast**: Notifications system for React.
- **react-redux**: Official React bindings for Redux.
- **react-router-dom**: Provides routing functionalities in React apps.
