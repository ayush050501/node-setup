# Node.js Setup Boilerplate

A robust and secure Node.js boilerplate built with Express.js, featuring integrated security, linting, and formatting tools. This repository provides a solid foundation for building scalable web applications and APIs.

## 🚀 Features

- **Framework**: Express.js for fast, unopinionated web development.
- **Security**: 
  - `helmet` for setting various HTTP headers (XSS Filter, Frameguard, CSP, HSTS, etc.).
  - `cookie-parser` for handling cookies.
  - `dotenv` for environment variable management.
- **Code Quality**:
  - `ESLint` with `airbnb-base` configuration.
  - `Prettier` for consistent code formatting.
  - `lint-staged` for running checks on staged files.
- **Project Structure**: Organized directory layout for routes, middlewares, services, and binaries.
- **Body Parsing**: Support for JSON and URL-encoded bodies with raw body capture.

## 🛠 Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [npm](https://www.npmjs.com/)

## 📦 Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd node-setup
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Environment Setup**:
   Create a `.env` file in the root directory and add your configuration variables.
   ```env
   PORT=3000
   ```

## 📜 Available Scripts

In the project directory, you can run:

| Command | Description |
| :--- | :--- |
| `npm start` | Runs the app in production mode. |
| `npm run lint` | Runs ESLint to find and fix code style issues. |
| `npm run format` | Runs Prettier to format all files. |
| `npm run check` | Checks if files are formatted according to Prettier rules. |
| `npm run lint:strict` | Runs ESLint and fails if there are any warnings. |

## 📂 Project Structure

```text
├── bin/            # Server entry point (www)
├── middlewares/    # Custom Express middlewares
├── public/         # Static assets (images, css, etc.)
├── routes/         # Express routes
├── services/       # Business logic and services
├── app.js          # Express application setup
├── package.json    # Project dependencies and scripts
└── README.md       # Project documentation
```

## 🔒 Security

This boilerplate uses `helmet` to help secure your Express apps by setting various HTTP headers.
- **CSP**: Content Security Policy is configured to allow self-hosted scripts and images.
- **HSTS**: HTTP Strict Transport Security is enabled for 1 year, including subdomains.
- **XSS Filter**: Enabled to prevent cross-site scripting attacks.
- **Frameguard**: Enabled to prevent clickjacking.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
