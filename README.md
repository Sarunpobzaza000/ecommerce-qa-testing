# E-Commerce QA Testing Project

Manual QA testing of the checkout flow on [SauceDemo](https://www.saucedemo.com/), a public practice e-commerce website. The project covers test planning, test case design, test execution, and bug reporting. Test automation is planned as the next phase.

## Project Status

🔄 **In Progress**: manual test execution

| Area | Test Cases | Executed | Passed | Failed |
|---|---|---|---|---|
| Login | 6 | 6 | 6 | 0 |
| Product Catalog | 8 | 8 | 8 | 0 |
| Shopping Cart | 5 | 0 | 0 | 0 |
| Checkout | 6 | 0 | 0 | 0 |
| **Total** | **25** | **14** | **14** | **0** |

## Testing Scope

**In scope**
- Login and error handling
- Product catalog: display, details, and sorting
- Shopping cart: add, remove, quantity, and price
- Checkout: information form, validation, order overview, and order completion

**Out of scope**
- Registration, product search, and real payment processing (these features are not part of SauceDemo)
- Performance, security, and cross-browser testing

See the full [Test Plan](test-plan/Test_Plan.md) for details.

## Testing Approach

- Functional testing
- Positive and negative testing
- Boundary testing
- Exploratory testing
- Regression testing

## Test Environment

| Item | Detail |
|---|---|
| Application | https://www.saucedemo.com/ |
| OS | Windows |
| Browser | Google Chrome |
| Test Account | `standard_user` (plus other SauceDemo accounts for bug finding) |

## Project Structure

```
ecommerce-qa-testing/
├── README.md
├── test-plan/
│   └── Test_Plan.md        # Scope, approach, environment, criteria, risks
├── test-cases/
│   └── Test_Cases.md       # 25 test cases with results
├── test-execution/         # Test execution results and summary report
├── bug-reports/            # Bug reports for failed test cases
├── screenshots/            # Test evidence
└── automation/             # Automated tests (planned)
```

## Deliverables

| Deliverable | Status |
|---|---|
| [Test Plan](test-plan/Test_Plan.md) | ✅ Done |
| [Test Cases](test-cases/Test_Cases.md) | ✅ Done (25 cases) |
| Test Execution | 🔄 In progress (14 of 25) |
| Bug Reports | ⏳ Planned |
| Test Summary Report | ⏳ Planned |
| Automated Tests | ⏳ Planned |

## Tools

- **Testing:** Google Chrome, manual testing
- **Documentation:** VS Code, Markdown
- **Version control:** Git, GitHub
- **Planned automation:** Python, Playwright, Pytest

## What I Learned

_To be completed at the end of the project._
