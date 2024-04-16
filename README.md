# Setup Process

The project was setup based on the following steps:

1. Installed NestJS CLI.
2. Initialized a NestJS app using `nest new dscdn-server`.
3. Selected `npm` as the package manager.
4. Installed initial dependencies to allow RestfulAPI funtionalities using `npm install @nestjs/platform-express`.
5. Started the development server using `npm run start:dev`.
6. Opened a web browser and navigated to `http://localhost:3000` to verify the application is running.

# Installation Instructions

To use this project, follow these steps:

1. Clone the repository on your selected local directory. "git clone <link>"
2. Install NestJS CLI globally `npm install -g @nestjs/cli` if you have not installed it on your computer.
3. Run `npm install` to install the dependencies.
4. Run `npm run start:dev` to start the server.
5. Open your web browser and go to `http://localhost:3000` to view the application.

# Project Structure

This codebase follows a typical structure for a NestJS application. Let's break it down:

## Root Directory

1. src/: Contains the main source code of the application
2. test/: Houses the end-to-end (e2e) tests
3. Configuration files:
- .gitignore: Specifies files and directories to be ignored by Git
- package.json: Defines project dependencies and scripts
- tsconfig.json: TypeScript compiler configuration
- nest-cli.json: NestJS CLI configuration
- .eslintrc.js: ESLint configuration for code linting
- .prettierrc: Prettier configuration for code formatting

## Source Directory 

1. main.ts: Entry point of the application, bootstraps the NestJS application
2. app.module.ts: Root module of the application
3. app.controller.ts: Main controller with route handlers
4. app.service.ts: Service layer for business logic
5. app.controller.spec.ts: Unit tests for the controller

## Test Directory

1. app.e2e-spec.ts: End-to-end tests for the application
2. jest-e2e.json: Jest configuration for e2e tests

The project follows a modular architecture, with the AppModule serving as the root module. The AppController handles incoming HTTP requests, while the AppService contains the business logic.

# Health Check Endpoint

The /health endpoint in `app.controller.ts` serves as a health check:

1. This endpoint allows monitoring systems to verify that the service is running and responsive. It returns a simple JSON response indicating the health status of the service.

Overall, this structure provides a solid foundation for building scalable and maintainable NestJS applications.
