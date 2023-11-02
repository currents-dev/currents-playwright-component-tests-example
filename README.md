# Playwright components testing with Currents

You can check the PW implementation [here](https://playwright.dev/docs/test-components)

First run `npm install`

For running the tests with PW only, you have to use `npm run test-ct` (This runs fine)

For running it with @currents/playwright `npx pwc --key <currentsKey> --project-id <projectId> --ci-build-id hello-currents`


The error showing right now when running with @currents/playwright is this:

```
SyntaxError: Unexpected token '<'

   at src/App.js:7

   5 |   return (
   6 |     <div className="App">
>  7 |       <header className="App-header">
     |                                    ^
   8 |         <img src={logo} className="App-logo" alt="logo" />
   9 |         <p>
  10 |           Edit <code>src/App.js</code> and save to reload.

    at Object.<anonymous> (/Users/miguelangarano/Documents/GitHub/pw-comps/src/App.js:7:36)
    at Object.<anonymous> (/Users/miguelangarano/Documents/GitHub/pw-comps/src/App.spec.js:4:35)

Error: No tests found







    ERROR  Global error reported by test runner: {
  message: "Unexpected token '<'",
  stack: "SyntaxError: Unexpected token '<'\n" +
    '    at Object.<anonymous> (/Users/miguelangarano/Documents/GitHub/pw-comps/src/App.js:7:36)\n' +
    '    at Object.<anonymous> (/Users/miguelangarano/Documents/GitHub/pw-comps/src/App.spec.js:4:35)',
  location: {
    file: '/Users/miguelangarano/Documents/GitHub/pw-comps/src/App.js',
    column: 36,
    line: 7
  },
  snippet: '\x1B[90m   at \x1B[39msrc/App.js:7\n' +
    '\n' +
    '\x1B[0m \x1B[90m  5 |\x1B[39m   \x1B[36mreturn\x1B[39m (\x1B[0m\n' +
    '\x1B[0m \x1B[90m  6 |\x1B[39m     \x1B[33m<\x1B[39m\x1B[33mdiv\x1B[39m className\x1B[33m=\x1B[39m\x1B[32m"App"\x1B[39m\x1B[33m>\x1B[39m\x1B[0m\n' +
    '\x1B[0m\x1B[31m\x1B[1m>\x1B[22m\x1B[39m\x1B[90m  7 |\x1B[39m       \x1B[33m<\x1B[39m\x1B[33mheader\x1B[39m className\x1B[33m=\x1B[39m\x1B[32m"App-header"\x1B[39m\x1B[33m>\x1B[39m\x1B[0m\n' +
    '\x1B[0m \x1B[90m    |\x1B[39m                                    \x1B[31m\x1B[1m^\x1B[22m\x1B[39m\x1B[0m\n' +
    '\x1B[0m \x1B[90m  8 |\x1B[39m         \x1B[33m<\x1B[39m\x1B[33mimg\x1B[39m src\x1B[33m=\x1B[39m{logo} className\x1B[33m=\x1B[39m\x1B[32m"App-logo"\x1B[39m alt\x1B[33m=\x1B[39m\x1B[32m"logo"\x1B[39m \x1B[33m/\x1B[39m\x1B[33m>\x1B[39m\x1B[0m\n' +
    '\x1B[0m \x1B[90m  9 |\x1B[39m         \x1B[33m<\x1B[39m\x1B[33mp\x1B[39m\x1B[33m>\x1B[39m\x1B[0m\n' +
    '\x1B[0m \x1B[90m 10 |\x1B[39m           \x1B[33mEdit\x1B[39m \x1B[33m<\x1B[39m\x1B[33mcode\x1B[39m\x1B[33m>\x1B[39msrc\x1B[33m/\x1B[39m\x1B[33mApp\x1B[39m\x1B[33m.\x1B[39mjs\x1B[33m<\x1B[39m\x1B[33m/\x1B[39m\x1B[33mcode\x1B[39m\x1B[33m>\x1B[39m and save to reload\x1B[33m.\x1B[39m\x1B[0m'
}
    ERROR  Global error reported by test runner: {
  message: 'No tests found',
  stack: 'Error: No tests found\n',
  location: undefined

================================================

    WARNING  No tests detected, skipping upload

================================================


```