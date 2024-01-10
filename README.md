# Go Hot Reload: A Go Web Application Template

## Introduction

Go Hot Reload is an open-source web application template using Go, designed to streamline the development process with hot reloading for HTML and Tailwind CSS. It's a perfect starting point for server side Go web development, particularly for those using `htmx`.

## Features

### Live Reloading 🔄

- **Go Code Rebuilding**: Automatic Go code rebuild using [`air`](https://github.com/cosmtrek/air). Configured in `.air.toml`.

### Hot Reloading 🔥

- **HTML Updates in Browser**: Dynamic HTML updates with [`reload`](https://github.com/aarol/reload). Injects JS for WebSocket updates.
- 🛠️ Uses `concurrently` npm package for running `air` and `npx tailwind` together. Details in `package.json`.

### HTML Templates 📄

- **Routing & Rendering**: [`chi`](https://github.com/go-chi/chi) router for serving HTML templates. 

### Tailwind 💅

- **Styling with [Tailwind](https://tailwindcss.com/)**: CSS framework for responsive, customizable UI components.

## Getting Started

### Setting Up the Environment

1. **Install npm Modules**: Run `npm install` to set up necessary modules.
2. **Environment Configuration**: Create a `.env` file with the following content:
   ```
   PORT=3000
   IS_DEVELOPMENT=true
   TEMPLATES_DIR=templates/
   STATIC_DIR=./static
   ```
3. **Launch the Development Server**: Start the server using `npm run dev`.
4. **Hot Reload**: Change the tailwind classes in `templates/landing.html` to see hot reload in action.

### Running Tests

The server includes an integration test.

- Execute tests using `go test ./...`.
- Or using npm command `npm run test`

## Contributing to Go Hot Reload

We welcome contributions from the community. Here are some guidelines to help you get started:

1. **Fork the Repository**: Start by forking the repository to your GitHub account.
2. **Clone Locally**: Clone your forked repository to your local machine.
3. **Create a New Branch**: Make your changes in a new git branch.
4. **Commit Your Changes**: Write meaningful commit messages that accurately describe your changes.
5. **Test Your Changes**: Ensure that your changes do not break any existing functionality.
6. **Submit a Pull Request**: Push your branch to your fork on GitHub and submit a pull request.

Thank you for considering to contribute to Go Hot Reload! Your efforts help make this project even better.
