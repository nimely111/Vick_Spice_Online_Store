# Vick_Spice_Online_Store

Tailwind CSS Course

Welcome to the Tailwind CSS course! This course will help you understand and use Tailwind CSS effectively for styling modern web applications.

Prerequisites

Before starting, ensure you have the following installed:

Node.js (Latest LTS recommended)

npm (Comes with Node.js)

Installation

To get started, install Tailwind CSS in your project:

npm install -D tailwindcss

Then initialize Tailwind CSS by running:

npx tailwindcss init

This will generate a tailwind.config.js file for customization.

Project Setup

Your project structure should look like this:

my-tailwind-project/
│── public/
│ ├── output.css
│── input.css
│── package.json
│── tailwind.config.js

Configure Tailwind

Add the following directive to your input.css file:

@tailwind base;
@tailwind components;
@tailwind utilities;

Running the Project

To generate the Tailwind CSS output file, use the following npm scripts:

Development Mode (Watch for Changes)

npm run watch

This command watches for changes in your input.css file and updates output.css automatically.

Build for Production

npm run build

This command compiles your Tailwind styles into output.css for production use.

Usage in HTML

Reference the compiled CSS file in your HTML file:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tailwind Course</title>
    <link href="./public/output.css" rel="stylesheet">
</head>
<body>
    <h1 class="text-3xl font-bold text-center text-blue-600">Welcome to Tailwind CSS!</h1>
</body>
</html>

Customization

Modify tailwind.config.js to customize Tailwind settings, such as themes, colors, and plugins.

Example:

module.exports = {
content: ["./*.html"],
theme: {
extend: {
colors: {
primary: "#1E40AF",
},
},
},
plugins: [],
};

Conclusion

You are now set up to build modern, responsive websites using Tailwind CSS! Happy coding!
