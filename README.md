# qBank Login Testing

Welcome to the **qBank Login Testing** repository! This project is focused on **manual testing** of the login functionality for the **qBank** website. The goal of this testing project is to ensure that the login feature works flawlessly, is secure, and offers a seamless user experience. 

## Table of Contents

- [Overview](#overview)
- [Test Objectives](#test-objectives)
- [Test Approach](#test-approach)
- [Test Cases](#test-cases)
  - [Positive Test Cases](#positive-test-cases)
  - [Negative Test Cases](#negative-test-cases)
- [Test Execution](#test-execution)
- [Bug Reports](#bug-reports)
- [Conclusion](#conclusion)
- [How to Run Tests](#how-to-run-tests)
- [Technologies Used](#technologies-used)

---

## Overview

This repository documents the testing of the **login functionality** on **https://qbank.accelq.com/**. It involves validating user login, security checks, and error handling mechanisms. The tests were conducted across **multiple browsers** (Chrome, Firefox, Safari) and **devices** (Desktop, Mobile) to ensure that the functionality is reliable and secure for all users.

## Test Objectives

The primary objectives of this testing project were to:

1. Validate that a user can log in with valid credentials.
2. Ensure that users cannot log in with invalid credentials (incorrect username/password).
3. Confirm that proper error messages are displayed when invalid data is entered.
4. Test the security of the login form (SQL injection).
5. Verify that the login page is responsive and works across different devices and browsers.

## Test Approach

### Manual Testing

- **Test Cases**: A set of 6 test cases covering both **positive** and **negative** scenarios were designed.
- **Browsers Tested**: Chrome, Firefox, Safari, Edge.
- **Devices Tested**: Desktop (Windows 10), Mobile (Android, iOS).
- **Security Tests**: SQL Injection testing was performed to ensure the login system is safe from common attacks.
- **UI/UX Testing**: The login form's responsiveness and alignment were checked on different screen sizes.

## Test Cases

### Positive Test Cases

1. **Valid Login**:  
   The user enters valid credentials (correct username and password) and successfully logs in.

2. **Password Masking**:  
   The password entered is properly masked with asterisks or dots to protect user privacy.

### Negative Test Cases

1. **Invalid Login - Incorrect Username**:  
   The user enters an incorrect username and a valid password, resulting in an error message.

2. **Invalid Login - Incorrect Password**:  
   The user enters a valid username and an incorrect password, triggering an error message.

3. **Empty Fields Validation**:  
   If the user leaves the username or password field empty, the system prompts the user to fill in both fields.

4. **SQL Injection Testing**:  
   The system is tested for vulnerabilities against SQL injection by attempting to log in with injection code like `' OR 1=1 --`. The system properly rejects the login attempt and does not allow unauthorized access.

---

## Test Execution

The tests were executed between **March 15, 2025** and **March 17, 2025**. Here are the test results:

- **Total Test Cases**: 6  
  - **Passed**: 6  
  - **Failed**: 0  
  - **Blocked**: 0  

All test cases passed successfully, confirming that the login functionality works as expected. No critical defects were found during testing, and the login system passed all the positive and negative test scenarios.

---

## Bug Reports

While conducting the tests, no major bugs or issues were found, except for a minor bug during the **Empty Fields Validation** test. The system didn't show an error message when the password field was left empty. This issue was noted and is being addressed by the development team.

---

## Conclusion

The **qBank login feature** has been tested thoroughly and passed all the necessary test cases. Both the **functionality** and **security** of the login page were validated, and no significant issues were encountered during the testing process.

### Key Takeaways:
- All test cases were executed successfully.
- The login system is secure and protected from SQL injection attacks.
- The login form is responsive and works well across different screen sizes and browsers.
- The system is ready for deployment with no critical issues remaining.

---

## How to Run Tests

1. **Clone this repository** to your local machine:
```bash
git clone * input my project link here *
```

2. **Install necessary testing tools** (e.g., browser drivers for Selenium, JIRA for bug tracking, etc.)

3. **Run the test cases manually** based on the instructions in the Test Cases section.

4. **Log any issues** found during testing in the **Bug Report** section for further review.

---

## Technologies Used

- **Manual Testing**
- **JIRA** for bug reporting
- **Browsers**: Chrome, Firefox, Safari
- **Devices**: Desktop (Windows 10), Mobile (Android/iOS)
- **Tools**: Word, Excel for test case documentation and execution logs

---

Feel free to explore this project and contribute any additional tests or improvements. Happy testing! 😊
