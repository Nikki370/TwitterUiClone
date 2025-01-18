# Twitter UI Clone

This project is a responsive clone of the Twitter user interface, created using Tailwind CSS. It demonstrates the use of Tailwind for rapid UI development, focusing on clean, maintainable, and customizable design.

## Features

- Fully responsive layout.
- Replicates the Twitter UI design.
- Built with Tailwind CSS for flexibility and customization.
- Easy to extend and adapt for additional features.

## Prerequisites

Ensure you have the following installed before setting up the project:

- Node.js (version 14 or above)
- npm (Node Package Manager)

## Installation

Follow these steps to set up the project locally:

1. Clone the repository:

    ```bash
    git clone <repository-url>
    cd twitter-ui-clone
    ```

2. Initialize the project:

    ```bash
    npm init -y
    ```

3. Install Tailwind CSS as a development dependency:

    ```bash
    npm install -D tailwindcss
    ```

4. Initialize the Tailwind CSS configuration:

    ```bash
    npx tailwindcss init
    ```

## Configuration

1. Open the  file and specify the paths to your HTML files:

    ```javascript
    module.exports = {
      content: ["./*.html"],
      theme: {
        extend: {},
      },
      plugins: [],
    };
    ```

2. Create a CSS file (`css/input.css`) and include Tailwind directives:

    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```

3. Add a build command in  under scripts:

    ```json
    "scripts": {
      "build": "npx tailwindcss -i ./css/input.css -o ./css/output.css --watch"
    }
    ```

## Usage

1. Run the Tailwind build process:

    ```bash
    npm run build
    ```

2. Include the generated  file in your :

    ```html
    <link href="css/output.css" rel="stylesheet">
    ```

3. Open  in your browser to view the Twitter UI clone.

## Project Structure

```plaintext
twitter-ui-clone/
│
├── css/
│   ├── input.css
│   ├── output.css
│
├── index.html
│
├── package.json
│
├── tailwind.config.js
│
└── node_modules/
