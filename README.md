# Playwright E2E Testing Project

Welcome to the Playwright E2E Testing project! This repository contains end-to-end tests using Playwright and TypeScript for a local web application. The application manages tasks with functionalities like Create, Read, Update, and Delete (CRUD). The application can be accessed locally at http://localhost:3000.

The WEB and API applications used in the tests were developed by Fernando Papito [linkedin](https://www.linkedin.com/in/papitoio/)

## Prerequisites

Before running the tests, ensure you have the following software installed on your system:

- [Node.js](https://nodejs.org/) version 18.10.0 or later
- [Yarn](https://yarnpkg.com/) (for dependency management)

## Getting Started

1. Clone this repository and navigate to the project folder:

    ```sh
    git clone <repository_url>
    cd playwright-sample
    ```

2. Install project dependencies using Yarn:

    ```sh
    yarn install
    ```

3. Start the target application locally:

    a. API:

    ```sh
    cd apps/api
    yarn install
    yarn db:init
    yarn dev
    ```

    b. Web:

    ```sh
    cd apps/web
    yarn install
    yarn dev
    ```

4. Run the end-to-end tests:

    ```sh
    yarn playwright test
    ```

   This command will execute the Playwright tests against the running web application.

## Structure

The project has the following structure:

- `apps/api`: API application for managing tasks
- `apps/web`: Web application for task management
- `tests`: Contains Playwright test scripts

## Contributing

Contributions are welcome! If you find any issues or improvements, please submit a pull request or create an issue.

## License

This project is licensed under the [MIT License](LICENSE).

