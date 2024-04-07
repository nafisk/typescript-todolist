# <img src='https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Typescript_logo_2020.svg/2048px-Typescript_logo_2020.svg.png' width='5%'> [Learning Journey: Complete TypeScript Project](https://youtu.be/61v23Ce5SXA?si=7FSQvv2NrBAnK333)

This project serves as a walkthrough for building a fully functional TypeScript application, aimed at understanding TypeScript's fundamentals through a practical project.

https://github.com/nafisk/typescript-todolist/assets/49691160/af4cc57c-24e8-4632-a968-0cf7f58eb538

## Setup

1. **Prerequisites:**

   - Node.js should be installed on the computer, ideally the "Recommended for most users" version, which at the time of this guide was `18.12.1`.
   - Visual Studio Code (VS Code) is recommended as the code editor for this project.

2. **Project Initialization:**

   - Opening a terminal in VS Code and checking the Node.js installation with `node -v` is a good first step.
   - A new project is created using Vite by executing `npm create vite@latest` in the terminal, following the setup prompts and selecting the `vanilla` option with TypeScript.

3. **Project Structure:**
   - Navigation to the new project directory is done (e.g., using `cd lesson11` for the project named `lesson11`).
   - `npm install` is run to install the necessary dependencies.
   - The development server is started with `npm run dev`.

## Development

1. **Creating the List Item Model:**

   - A `model` directory is created within the `src` directory.
   - Inside `model`, a `listItem.ts` file is created.
   - An `Item` interface is defined with properties: `id` (string), `item` (string), and `checked` (boolean).
   - A `ListItem` class is implemented with private variables and their corresponding getters and setters.

2. **Building the Full List Model:**

   - In the `model` directory, a `fullList.ts` file is created.
   - `ListItem` is imported, and a `FullList` class is defined, implementing operations such as `load`, `save`, `clear`, `addItem`, and `removeItem`.

3. **Creating the List Template:**

   - A `templates` directory is created in the `src` directory.
   - Within `templates`, a `listTemplate.ts` file is created.
   - The `ListTemplate` class is implemented to handle the rendering of the list in the DOM, including methods for clearing and rendering the list items.

4. **Integrating Models and Templates into the Main Application:**
   - The `main.ts` file imports the necessary models and templates.
   - The application is initialized, event listeners are set up, and logic is implemented to add, remove, and display list items.

## Running the Application

- `npm run dev` is used to start the development server.
- The application is accessed at `localhost:5173` in a web browser to view and interact with it.
- Functionality is tested by adding, checking off, deleting, and clearing list items.

**Learning Note:** Emphasis is placed on progress over perfection, with the understanding that consistent, small steps lead to significant learning achievements over time.
