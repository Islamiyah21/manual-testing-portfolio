# Manual Testing Scenarios — Sample Banking Application

## 1. Project Overview

This project demonstrates manual testing techniques using a fictional mobile banking application.

The application allows users to log in, view account balances, and transfer funds to beneficiaries.

**Testing Type:** Manual Functional Testing

**Application:** Fictional Mobile Banking Application

**Objective:** To verify that key banking features behave as expected and that invalid inputs and error conditions are handled appropriately.

## 2. Login Testing

| Test ID   | Test Scenario                                | Expected Result                                   |
| --------- | -------------------------------------------- | ------------------------------------------------- |
| LOGIN-001 | Log in with valid credentials                | The user should log in successfully.              |
| LOGIN-002 | Log in with an incorrect password            | An appropriate error message should be displayed. |
| LOGIN-003 | Submit the login form with an empty username | The username should be identified as required.    |
| LOGIN-004 | Submit the login form with an empty password | The password should be identified as required.    |
| LOGIN-005 | Submit the login form with both fields empty | Required-field validation should be displayed.    |

## 3. Account Balance Testing

| Test ID | Test Scenario                                    | Expected Result                                              |
| ------- | ------------------------------------------------ | ------------------------------------------------------------ |
| BAL-001 | View the account balance after logging in        | The account balance should be displayed correctly.           |
| BAL-002 | Refresh the account balance                      | The application should display the latest available balance. |
| BAL-003 | Attempt to view an account without authorization | Access should be denied.                                     |

## 4. Fund Transfer Testing

| Test ID   | Test Scenario                                          | Expected Result                                                 |
| --------- | ------------------------------------------------------ | --------------------------------------------------------------- |
| TRANS-001 | Transfer funds to a valid beneficiary                  | The transfer should be processed successfully.                  |
| TRANS-002 | Attempt a transfer with insufficient funds             | The transfer should be rejected with an appropriate message.    |
| TRANS-003 | Enter an invalid beneficiary account number            | The application should validate the account details.            |
| TRANS-004 | Submit a transfer with an empty amount                 | The amount field should be validated.                           |
| TRANS-005 | Enter a zero or negative transfer amount               | The application should reject an invalid amount.                |
| TRANS-006 | Attempt to submit the same transfer repeatedly         | The application should prevent unintended duplicate transfers.  |
| TRANS-007 | Review the account balance after a successful transfer | The balance should reflect the completed transaction correctly. |

## 5. Security and Session Testing

| Test ID | Test Scenario                                              | Expected Result                                                 |
| ------- | ---------------------------------------------------------- | --------------------------------------------------------------- |
| SEC-001 | Attempt to access an authenticated page without logging in | The application should require authentication.                  |
| SEC-002 | Log out and attempt to return to an authenticated page     | The application should prevent access to protected information. |
| SEC-003 | Leave a session inactive for the configured timeout period | The application should handle session expiry appropriately.     |

## 6. Testing Notes

* These are proposed test scenarios for a fictional application.
* No live banking application has been tested as part of this document.
* Actual results and defect status should only be recorded after executing tests against an available test environment.
* Financial transactions must be tested only in an authorized test environment using approved test data.

## 7. Conclusion

These scenarios provide a starting point for validating the login, account balance, fund transfer, and session management features of a banking application.

Additional test cases should be developed from approved requirements and executed in a suitable test environment.
