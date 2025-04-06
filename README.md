API Node TDD Clean
Description
This project is an implementation of an API in Node.js following the principles of Test-Driven Development (TDD) and Clean Architecture.

The goal of the project is to create a robust, scalable, and maintainable system by focusing on clean code practices and ensuring that all business logic is thoroughly tested. It leverages TypeScript and Node.js to build a clean, well-structured, and testable API.

Features
Test-Driven Development (TDD): All features are built and tested with TDD methodology to ensure code quality.

Clean Architecture: Structured using clean architecture principles to separate concerns and make the codebase easy to maintain and extend.

Node.js & Express: Backend API built using Node.js and Express framework.

TypeScript: Full TypeScript support for type safety and better development experience.

Jest: Testing framework used to ensure the application is thoroughly tested.

Database: (Insert database technology here, e.g., PostgreSQL, MongoDB, etc.)

Installation
Prerequisites
Before running the application, make sure you have the following installed:

Node.js (>=12.0.0)

npm or yarn (for package management)

PostgreSQL (or another database, if applicable)

Steps
Clone the repository:
git clone https://github.com/luizcurti/api-node-TDD-clean.git
Navigate to the project directory:
cd api-node-TDD-clean
Install dependencies:
npm install
# Or if you are using Yarn:
yarn install
Set up environment variables:

Create a .env file at the root of the project and add your environment variables. You can use .env.example as a reference.

DATABASE_URL=your_database_url
PORT=your_app_port

Run the application:
npm start
# Or with Yarn:
yarn start
The API will be available at http://localhost:3000 (or whichever port you specified).

Running Tests
To run the tests and ensure that everything is working correctly, use the following command:
npm test
# Or with Yarn:
yarn test
This will run all the unit tests and integration tests to ensure the application behaves as expected.

Running Linter
To check the code for any linting issues:
npm run lint
# Or with Yarn:
yarn lint

Folder Structure
The project follows Clean Architecture principles, which ensure that business logic is decoupled from the frameworks and tools.

.
├── src
│   ├── config          # Configuration files (e.g., database, server settings)
│   ├── modules         # Core business logic
│   │   ├── user        # Example module (User)
│   │   │   ├── domain  # Domain models, entities, and value objects
│   │   │   ├── use-cases # Use cases or business logic
│   │   │   ├── infra    # Infra layer: repository implementations, DB queries
│   │   │   └── presentation # Controllers, Routes
│   ├── shared          # Shared modules and utilities
│   ├── tests           # Unit and integration tests
└── .env                # Environment variables
└── .gitignore          # Git ignore file
└── jest.config.js      # Jest configuration
└── tsconfig.json       # TypeScript configuration
└── package.json        # Project metadata and dependencies

Technologies Used
Node.js: Runtime environment to build the API.
Express: Web framework for building the API.
TypeScript: Superset of JavaScript that allows for static typing.
Jest: Testing framework to write unit and integration tests.
ESLint/Prettier: Tools for code linting and formatting.
Sequelize (or other ORM): ORM for interacting with the database (or another ORM if applicable).
PostgreSQL (or other database): Database to store data.

Testing
The application follows the Test-Driven Development (TDD) approach. Tests are written first, and the code is implemented to make the tests pass. This ensures that the system behaves as expected.

Running Tests
To run the tests:
npm test
# Or with Yarn:
yarn test

Test Coverage
You can check the test coverage report by running:

npm run coverage
# Or with Yarn:
yarn coverage
