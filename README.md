# Cypress Testing Project

This repository contains automated end-to-end tests built with Cypress.  
It’s a practice and learning project to explore writing, running, and managing Cypress tests.

## Project Overview

- Framework: Cypress  
- Language: JavaScript  
- Folder structure:
  cypress/
├── e2e/ # Test files (.cy.js)
├── fixtures/ # Test data
└── support/ # Commands and setup


---

## Setup Instructions

1. Clone the repository
   
'bash'

 git clone ; https://github.com/UmarImranQA/cypress-automation-tests.git
 
 cd cyprress-automation-tests

2. Install dependencies

'bash'

npm install


3. Open Cypress Test Runner (interactive)
   
'bash'

npx cypress open


5. Run tests in headless mode (for CI)

'bash'

npx cypress run


## Writing Tests

All test files live inside cypress/e2e/.

example;

'js'

describe('My First Test', () => {
  it('Visits the Cypress docs', () => {
    cy.visit('https://docs.cypress.io')
    cy.contains('Testing').should('exist')
  })
})


## Git Workflow

Default branch: main

Branch naming suggestion: feature/<name> or test/<name>

Example:

git checkout -b test/login-flow

## Troubleshooting & Maintenance

--If Cypress binaries or cache cause issues:

'bash'

npx cypress cache clear

npx cypress install


--If you need to upgrade Cypress:

'bash'

npm uninstall cypress

npm install cypress@latest --save-dev

npx cypress install


## Dependencies

Node.js

Cypress

## Author

Umar Imran

Quality Assurance Engineer in training

GitHub: https://github.com/UmarImranQA
