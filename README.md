# Lab 9 - Starter

**Published GitHub Pages URL:**  https://rena-tokhi.github.io/Lab9_Starter/


## What this lab demonstrates

### Step 2 — Console API (the 15 buttons)
Each button calls a different `console` method:
- Console Log — plain + `%c` styled log
- Console Error — error-styled message
- Console Count — increments a named counter each click
- Console Warn — warning-styled message
- Console Assert — prints only when the assertion is false
- Console Clear — clears the console
- Console Dir — interactive property listing of a DOM node
- Console dirxml — HTML/XML tree of a node
- Console Group Start / Console Group End — opens/closes an indented group
- Console Table — array of objects as a sortable table
- Start Timer / End Timer — `console.time` / `console.timeEnd`
- Console Trace — prints the call stack
- Trigger a Global Error — Step 5 (see below)

### Step 3 — try / catch / finally
The Error Calculator's submit handler wraps the calculation in
try/catch/finally. Bad input is caught and shown in the `<output>`;
the `finally` block always logs that the attempt finished.

### Step 4 — throw & custom errors
`CalculatorError extends Error`. The calculator throws it for empty
fields, non-numeric input, and divide-by-zero, then the catch block
displays `err.name: err.message`.

### Step 5 — Global error handler & TrackJS
`window.onerror`, `window.addEventListener('error')`, and
`unhandledrejection` catch errors that escape try/catch. The "Trigger
a Global Error" button calls an undefined function so the error reaches
global scope and is logged.

**To enable TrackJS:** uncomment the snippet in `<head>`, paste your
trial token, reload, click "Trigger a Global Error" a few times, then
add a dashboard screenshot (showing your username + error list) under
`screenshots/`.

## Run locally
Open `index.html` and open DevTools (F12) to watch the console.