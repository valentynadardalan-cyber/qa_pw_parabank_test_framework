# Task Description

To see the description of the task assignment [follow the link](https://github.com/mate-academy/qa_pw_parabank_test_framework/blob/main/TaskDescription.md). 

# Repository Overview

This repository contains a test automation framework for the [Parabank](https://parabank.parasoft.com/parabank/index.htm) bank application testing. 

# How to use this project

## Installation steps

To install the project follow the next steps:

1. Install Node.js.
2. Run the installation command in the project root.:
```bash
npm ci
```
3. Run the browsers installation in the project root.
```bash
npx playwright install
```
4. Install Allure commandline tool (Allure requires Java 8 or higher).
```bash
npm install -g allure-commandline
```

## How to run the tests

Before running the tests, make sure that the Parabank Administration page
uses the following settings:

The loan tests automatically configure the required Parabank administration
settings before requesting a loan.

Do not use the `Clean` or `Initialize` database actions while the tests are
running.

Run all tests:

```bash
npm test
```

Run tests in headed mode:

```bash
npm run test:headed
```

Run tests in Playwright UI mode:

```bash
npm run test:ui
```

Run a specific test file:

```bash
npx playwright test path/to/test.spec.js
```

Run the code-style check:

```bash
npm run lint
```

## How to generate report

Test execution creates Allure results in the `allure-results` directory.

Generate the Allure HTML report:

```bash
npm run report:generate
```

Open the generated report:

```bash
npm run report:open
```

The generated report is stored in the `allure-report` directory.