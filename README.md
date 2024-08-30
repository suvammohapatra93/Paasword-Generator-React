# Random Password Generator

This project is a simple web application that generates random passwords. You can generate passwords composed of numbers or words, and you have the option to set the length of the password. The project is built with React and Vite, using Tailwind CSS for styling.

## Features

- **Random Password Generation**: Generate secure random passwords.
- **Password Types**: Choose between numeric passwords or word-based passwords.
- **Custom Length**: Set the length of your password to your desired number of characters.

## Tech Stack

- **React**: A JavaScript library for building user interfaces.
- **Vite**: A fast development build tool and dev server for modern web projects.
- **Tailwind CSS**: A utility-first CSS framework for designing custom UI components.
- **JavaScript (JS)**: The programming language used to handle the logic of the application.
- **CSS**: For styling the application.
- **HTML**: The standard markup language used to structure the content of the app.

### Built With

React
Vite
Tailwind CSS

### Prerequisites

Before running the project, make sure you have the following installed:

Node.js: JavaScript runtime
npm or yarn: Package manager

### Running this Project

1. **Create a Vite project**: 

    ```bash
    npm create vite@latest
    ```

    This command sets up a new Vite project. You'll be prompted to enter a project name and select a template (e.g., React). 

2. **Navigate to the project directory**:

    ```bash
    cd your-project-name
    ```

    Replace `your-project-name` with the actual name of the directory created by the Vite setup.

3. **Install project dependencies**:

    ```bash
    npm install
    ```

    This installs the project dependencies defined in the `package.json` file.

4. **Install Tailwind CSS and related tools**:

    ```bash
    npm install -D tailwindcss postcss autoprefixer
    ```

    This installs Tailwind CSS along with PostCSS and Autoprefixer, which are needed for processing Tailwind CSS.

5. **Initialize Tailwind CSS**:

    ```bash
    npx tailwindcss init -p
    ```

    This command creates a `tailwind.config.js` file and a `postcss.config.js` file with default configurations for Tailwind CSS and PostCSS.

6. **Configure Tailwind CSS**: 

    Edit the `tailwind.config.js` file to include the paths to your HTML and JavaScript files:

    ```javascript
    /** @type {import('tailwindcss').Config} */
    export default {
      content: [
        "./index.html",
        "./src/**/*.{js,ts,jsx,tsx}",
      ],
      theme: {
        extend: {},
      },
      plugins: [],
    }
    ```

    This ensures Tailwind CSS processes all the necessary files in your project.

7. **Add Tailwind directives to your CSS**:

    Update `index.css` (or whichever CSS file you are using) to include Tailwind’s base, components, and utilities:

    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```

    This imports Tailwind CSS’s default styles into your project.

8. **Start the development server**:

    ```bash
    npm run dev
    ```

    This starts the Vite development server and opens the application in your default web browser.

## Building for Production

To create an optimized build for production:

```bash
npm run build
# or if you use yarn
yarn build