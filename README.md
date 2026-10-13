# React Todo App

A React application for browsing todos from a public API. Search tasks by title,
filter them by completion status, and view task details and owner information.

## Live Preview

[View on GitHub Pages](https://ievgen-nikiforov.github.io/react-todo-app/)

## Technologies Used

- **React 18 and TypeScript** — components and typed application logic.
- **Redux Toolkit and React Redux** — shared state for todos, filters, and the
  selected task.
- **Vite** — development server and production bundling.
- **Bulma and SCSS** — layout and styling.
- **Font Awesome** — interface icons.
- **Fetch API** — loading todos and user details.

## Getting Started

### Prerequisites

- Node.js 20 and npm.
- Git to clone the repository, or download and extract its ZIP archive.
- An internet connection to install dependencies and load the public API data.

### Installation

1. Clone the repository and enter the project folder:

   ```sh
   git clone https://github.com/ievgen-nikiforov/react-todo-app.git
   cd react-todo-app
   ```

2. Install the locked dependencies:

   ```sh
   npm ci
   ```

3. Start the development server:

   ```sh
   npm start
   ```

   Open the local URL printed in the terminal. No API key or environment
   variables are required.

### Available Commands

| Command            | Description                                                |
| ------------------ | ---------------------------------------------------------- |
| `npm start`        | Start the local development server.                        |
| `npm run build`    | Create a production build.                                 |
| `npm run lint-js`  | Check JavaScript and TypeScript code.                      |
| `npm run lint-css` | Check SCSS styles.                                         |
| `npm run format`   | Format TypeScript source files.                            |
| `npm run lint`     | Format source files and styles, then run both lint checks. |

## Features

- Load and display todos from a public API.
- Filter tasks by **All**, **Active**, or **Completed** status.
- Search titles without case sensitivity and clear the search with one click.
- Combine status and search filters.
- Open a task details modal showing its ID, title, status, and owner's name.
- Contact a task owner through an email link.
- Display loading indicators and a message when no tasks match the filters.

## Project Structure

```text
src/
  api.ts          # Requests for todos and users
  app/            # Redux store and typed hooks
  components/     # Todo list, filters, details modal, and loader
  features/       # Redux slices for todos, filters, and selection
  types/          # Todo, user, and status types
  App.tsx         # Main application component
  index.tsx       # Application entry point
```
