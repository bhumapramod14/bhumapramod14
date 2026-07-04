# MeeBhoomi Automation

## Overview

This project automates the MeeBhoomi website using Playwright.

## Technologies Used

- Playwright
- JavaScript
- Node.js

## Project Files

- `src/login.spec.js` – Login automation.
- `tests/index.spec.js` – Main automation script.

## How to Run

Install dependencies:

```bash
npm install
```

Run the login script:

```bash
npx playwright test src/login.spec.js
```

Run the main automation:

```bash
npx playwright test tests/index.spec.js
```

## Challenges

- OTP and CAPTCHA need to be entered manually.
- After submitting the search request, the website keeps showing **"Loading... Please Wait"** in Playwright.
- In a normal browser, the same request returns **"No Data Found"**.

## Notes

- OTP verification and CAPTCHA require manual input during execution because they are dynamic.
- The automation was developed using Playwright.
- During testing, the MeeBhoomi portal remained on "Loading... Please Wait" after the search request in the Playwright browser, while the same request returned "No Data Found" in a normal Chrome browser.