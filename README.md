# Playwright components testing with Currents

Run [Playwright component](https://playwright.dev/docs/test-components) tests and report the results to [Currents](https://currents.dev)

> **Note: November 2023** Playwright support for Components Testing is still experimental

The project contains simple component tests:

- `src/App.spec.jsx` - a passing test
- `src/AppFailing.spec.jsx` - a failing test

## Setup

- First run `npm i`
- Create an account and project at https://app.currents.dev
- Grab the following details:
  - `projectId`
  - `recordKey`

## Run

Run `pwc` command:

`npx pwc --key <recordKey> --project-id <projectId> --ci-build-id hello-currents`

- Explore `playwright-ct.config.js` and note that screenshots, videos and trace are activated
- Explore more about [CI Build Id](https://currents.dev/readme/guides/cypress-ci-build-id)

Running the command would produce an output that is similar to this:

The reported results in Currents Dashboard, please note the failed tests:

## Explore `@currents/playwright` integration options

Follow our documentation to explore integration options:
https://currents.dev/readme/integration-with-playwright/currents-playwright
