# E-Commerce QA Testing — Test Plan

| Item | Detail |
|---|---|
| **Project** | E-Commerce Checkout Flow — Manual QA Testing |
| **Application Under Test** | [SauceDemo](https://www.saucedemo.com/) (Swag Labs demo store) |
| **Prepared by** | Pob |
| **Document Status** | In Progress |

---

## 1. Introduction

This test plan describes how the SauceDemo e-commerce website will be tested. The main focus is the checkout flow: a user logs in, browses products, manages the shopping cart, and completes an order.

SauceDemo is a public practice website made for software testing. It includes several test accounts, some of which contain intentional defects, which makes it suitable for practicing defect discovery and bug reporting.

## 2. Objectives

- Verify that the main user flow (login → products → cart → checkout → order complete) works correctly.
- Verify that the application handles invalid and missing input correctly.
- Find, document, and report defects clearly and reproducibly.
- Record test results with evidence (screenshots).
- Automate the most important test cases after manual testing is complete.

## 3. Scope

### 3.1 In Scope

| Area | What will be tested |
|---|---|
| **Login** | Valid login, invalid username, invalid password, missing fields, error messages |
| **Product Catalog** | Product display, product details, sorting (name and price), add/remove from the Products page |
| **Shopping Cart** | Product information, quantity, price, removing items, Continue Shopping, Checkout button, cart badge updates |
| **Checkout** | Checkout information form, required-field validation, Checkout Overview (subtotal, tax, total), order completion |

### 3.2 Out of Scope

These features do not exist on SauceDemo, so they will not be tested:

- User registration and account creation
- Product search
- Real payment processing (SauceDemo uses a fake payment step)
- Order history and email confirmation

These areas are also out of scope for this project:

- Performance and load testing
- Security and penetration testing
- Mobile app testing
- Cross-browser testing (only Google Chrome is used)

## 4. Test Environment

| Item | Detail |
|---|---|
| **URL** | https://www.saucedemo.com/ |
| **Operating System** | Windows |
| **Browser** | Google Chrome (latest version) |
| **Documentation Tools** | VS Code, Markdown |
| **Version Control** | Git and GitHub |
| **Screenshot Tool** | Windows Snipping Tool |

## 5. Test Accounts

All accounts use the password `secret_sauce`.

| Username | Purpose |
|---|---|
| `standard_user` | Normal user. Main account for functional testing. |
| `locked_out_user` | Locked account. Used to test login rejection. |
| `problem_user` | Account with intentional UI and functional defects. Used to find bugs. |
| `performance_glitch_user` | Account with slow responses. Used to observe delays. |
| `error_user` | Account that triggers errors in some actions. Used to find bugs. |
| `visual_user` | Account with visual differences. Used for visual and layout checks. |

## 6. Test Approach

### 6.1 Test Types

| Type | How it is applied |
|---|---|
| **Functional testing** | Check that each feature works as expected. |
| **Positive testing** | Use valid input and check for the correct result. |
| **Negative testing** | Use invalid or missing input and check that it is rejected with a clear message. |
| **Boundary testing** | Test edge cases, such as an empty cart or very long input in checkout fields. |
| **Exploratory testing** | Use the site freely, especially with `problem_user` and `error_user`, to find unexpected issues. |
| **Regression testing** | Re-run earlier test cases after a change or a fix to confirm nothing else broke. |

### 6.2 Process

1. Write test cases in `test-cases/Test_Cases.md`.
2. Run each test case manually in Chrome.
3. Record the **Actual Result** and the **Status** (PASS, FAIL, or BLOCKED).
4. Take screenshots as evidence and save them in `screenshots/`.
5. Report every FAIL as a bug in `bug-reports/`.
6. Summarize the results in `test-execution/`.

### 6.3 Test Case Coverage

| Area | ID Prefix | Number of Test Cases |
|---|---|---|
| Login | TC-LOGIN | 6 |
| Product Catalog | TC-PRODUCT | 8 |
| Shopping Cart | TC-CART | 5 |
| Checkout | TC-CHECKOUT | 6 |
| **Total** | | **25** |

## 7. Entry and Exit Criteria

### 7.1 Entry Criteria (when testing can start)

- The SauceDemo website is available and loads in Chrome.
- The test accounts can be used.
- Test cases have been written and reviewed.

### 7.2 Exit Criteria (when testing is finished)

- All 25 test cases have been run.
- Every failed test case has a bug report.
- All test results and evidence have been committed to GitHub.
- The Test Summary Report is complete.

## 8. Defect Management

Each bug report in `bug-reports/` will include:

- **Bug ID** (for example, BUG-001)
- **Title** (a short summary)
- **Related Test Case ID**
- **Environment** (browser, OS, test account)
- **Steps to Reproduce**
- **Expected Result** and **Actual Result**
- **Severity**: Critical, High, Medium, or Low
- **Priority**: High, Medium, or Low
- **Evidence** (a screenshot or a screen recording)

### Severity Levels

| Severity | Meaning | Example |
|---|---|---|
| **Critical** | The main flow is blocked. | The user cannot complete an order. |
| **High** | A major feature works incorrectly. | The cart total is calculated wrong. |
| **Medium** | A feature has a problem, but a workaround exists. | Sorting shows products in the wrong order. |
| **Low** | A cosmetic or minor issue. | A misaligned button or a typo. |

## 9. Deliverables

| Deliverable | Location | Status |
|---|---|---|
| Test Plan | `test-plan/Test_Plan.md` | ✅ Done |
| Test Cases | `test-cases/Test_Cases.md` | ✅ Done (25 cases) |
| Test Execution Results | `test-execution/` | 🔄 In progress |
| Screenshots and Evidence | `screenshots/` | ⏳ Not started |
| Bug Reports | `bug-reports/` | ⏳ Not started |
| Test Summary Report | `test-execution/` | ⏳ Not started |
| Automated Tests | `automation/` | ⏳ Not started |

## 10. Risks and Mitigation

| Risk | Mitigation |
|---|---|
| SauceDemo is a public demo site and may be down or change without notice. | Record the test date and take screenshots as evidence. |
| `standard_user` has no intentional bugs, so most tests may pass. | Repeat key tests with `problem_user` and `error_user` to find real defects. |
| Manual testing can lead to mistakes in recording results. | Write exactly what is seen on screen and attach a screenshot. |
| Test data can carry over between tests (for example, items left in the cart). | Reset the app state (menu → Reset App State) or log out before each test. |

## 11. Future Work: Test Automation

After manual testing is complete, the most important test cases (login, add to cart, and complete checkout) will be automated with:

- **Python**
- **Playwright**
- **Pytest**

Automated tests will be stored in the `automation/` folder.
