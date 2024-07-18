# Automation-With-Cypress
his repository contains a Cypress project for automated testing of the SauceDemo website.

## Project Structure

- `cypress`
  - `e2e`
    - `TestSpec.cy.js`: Contains the test specifications.
  - `pages`
    - `HomePage.js`: Contains methods for interacting with the home page.
    - `LoginPage.js`: Contains methods for interacting with the login page.
    - `ProductPage.js`: Contains methods for interacting with the product page.
  - `reports`
    - `mochawesome.json`: JSON report generated by Mochawesome.
    - `mochawesome.html`: HTML report generated by Mochawesome.
- `node_modules`: Contains project dependencies.
- `cypress.config.js`: Cypress configuration file.
- `package.json`: Project's package file.
- `package-lock.json`: Automatically generated file that contains the exact versions of dependencies.

## Custom Commands and Page Object Model (POM)

### Custom Commands

Reusable test steps are defined as custom commands in Cypress. These commands can be found in the `commands.js` file (if applicable).

### Page Object Model

This project follows the Page Object Model (POM) pattern, with separate classes for each page:

- `LoginPage`: Handles actions related to the login page.
- `HomePage`: Handles actions related to the home page.
- `ProductPage`: Handles actions related to the product page.

## Test Cases

The test cases are defined in `TestSpec.cy.js`:

- **Wrong Login**: Attempts a wrong login and verifies the error message.
- **Login and Home Page**: Logs into the app and verifies that the user lands on the home page.
- **Product Page Navigation**: Clicks on a product and verifies that the browser navigates to the product page.

## Setup and Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/Ass1Cypress.git
   cd Ass1Cypress

2. **Install dependencies:**
   ```bash
   npm install

3. **To run the Cypress tests, execute the following command:**
   ```bash
   npm run cypress:run
   
4. **Generating Reports:**
   ```bash
   npm run test:report


