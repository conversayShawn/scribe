# Support Team Sandbox
Based on [cypress-test-tiny](https://github.com/cypress-io/cypress-test-tiny)

This is a small project for quickly reproducing customer issues.

You can find instructions for common setups or CI Providers on the designated branch:
- AWS Codebuild [WIP]
- Buildkite [WIP]
- CircleCI [WIP]
- [Cucumber](https://github.com/conversayShawn/scribe)
- GitHub Actions [WIP]
- Jenkins [WIP]
- Travis [WIP]


_Note_ If a CI Provider is missing or needs to be updated, submit a request form here: [Form]() 


## IMPORTANT

This project DOES NOT include the following:
- Package manager
- Cypress dependency in the `package.json`

Installation
```
# PACKAGE MANAGER
npm init or yarn init or pnpm init
# CYPRESS
npm i -D cypress or npm i -D cypress@x.x.x (Be sure to use the same command as your package manager)
```

 The reason for such omission is that we use this project to test every Cypress build and do not want to spend time installing cypress@x.x.x just to immediately install and test cypress@y.y.y. Which means when submitting pull requests with a bug report, please save the problematic version of Cypress in package.json. Simply run npm install --save-dev cypress or npm i -D cypress@x.x.x and commit the change before submitting a pull request.