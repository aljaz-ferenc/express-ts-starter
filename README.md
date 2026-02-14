# Express + TypeScript Starter

A minimal, production-ready Express.js starter with TypeScript support.

## Includes

- **Express with TypeScript** - Type-safe server development
- **Environment Variables** - dotenv for configuration management
- **Hot Reload** - Nodemon for development
- **Code Quality** - Biome for linting and formatting
- **Git Hooks** - Husky pre-commit integration
- **Project Structure** - Organized and scalable folder layout
- **Error Handling** - Process-level error handling and graceful shutdown

## Getting Started

### Prerequisites

- Node.js
- pnpm (recommended) or npm

### Installation

1. Clone the repository:
2. Install dependencies
```
pnpm install
```
3. Create a `.env` file in the project root
```
PORT=4000
```

Here you go:

### Scripts

- **`pnpm dev`** - Runs the development server with hot reload using nodemon in development environment
- **`pnpm start`** - Starts the production server from the compiled `dist` folder
- **`pnpm build`** - Compiles TypeScript to JavaScript
- **`pnpm prebuild`** - Automatically runs before `build` to clean/remove the `dist` folder
- **`pnpm prepare`** - Sets up Husky git hooks (runs automatically after package installation)
- **`pnpm check`** - Runs Biome to lint, format, and auto-fix code issues

### Project Structure
```
src/
├── app.ts            # Express app configuration
├── index.ts          # Server entry point
├── error-handlers.ts # Global error handling
├── controllers/      # Route controllers / request handlers
├── routes/           # API route definitions
├── services/         # Business logic layer
├── middleware/       # Custom Express middleware
```