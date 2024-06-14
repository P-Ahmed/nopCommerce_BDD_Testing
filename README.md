```markdown
# Automated Testing for NopCommerce Features

## Introduction

We aim to build an automation project that executes every night at 12:00 AM, generates reports, and provides them. Currently, we want to cover two features: Registration and PlaceOrder.

Website link: [nopCommerce](https://demo.nopcommerce.com/)

## Registration Feature

### Scenario: User Registration

1. **Given** the user is on the NopCommerce Home page.
2. **And** the user navigates to the Registration page.
3. **When** the user selects the gender as `<type>`.
4. **And** the user sets the first name and last name.
5. **And** the user sets the date of birth as `<dob>`.
6. **And** the user sets the email as `<dynamicEmail>`.
7. **And** the user sets the company details as `<companyName>`.
8. **And** the user sets the newsletter option as `<status>`.
9. **And** the user sets the password and confirms it.
10. **And** the user clicks on the Register button.
11. **Then** verify that the new account registration message `<msg>` is displayed.

### Examples:

| type     | dob          | dynamicEmail | companyName       | status      | password    | msg                           |
| -------- | ------------ | ------------ | ----------------- | ----------- | ----------- | ------------------------------ |
| "Male"   | "20/05/1995" | ""           | "Ahmed Pvt. Ltd." | "checked"   | "pass@1234" | "Your registration completed" |
| "Female" | "9/05/1999"  | ""           | "Ahmed Pvt. Ltd." | "unchecked" | "pass@1234" | "Your registration completed" |
| "Female" | "3/05/2000"  | ""           | "Ahmed Pvt. Ltd." | "unchecked" | "pass@1234" | "Your registration completed" |
| "Male"   | "2/05/2001"  | ""           | "Ahmed Pvt. Ltd." | "checked"   | "pass@1234" | "Your registration completed" |
| "Female" | "10/05/1990" | ""           | "Ahmed Pvt. Ltd." | "unchecked" | "pass@1234" | "Your registration completed" |

## PlaceOrder Feature

### Scenario: Placing an Order as a Guest User

1. **Given** the user is on the NopCommerce Home page.
2. **When** the user clicks on "Cell phones" under the "Electronics" category.
3. **And** the user selects the "Nokia Lumia 1020" for product details.
4. **And** the user sets the quantity to 2.
5. **And** the user clicks the "ADD TO CART" button.
6. **And** the user proceeds to the shipping cart page.
7. **And** the user accepts the terms and conditions and clicks the checkout button.
8. **And** the user checks out as a guest.
9. **And** the user inputs billing details and clicks continue.
10. **And** the user selects the shipping method as "Next Day Air" and clicks continue.
11. **And** the user selects the payment method as "Credit Card" and clicks continue.
12. **And** the user selects the "Visa" card and inputs card information.
13. **And** the user clicks the confirm button to place the order.
14. **Then** verify that the order placement message "Your order has been successfully processed!" is displayed.

## Additional Functionalities

- Automation projects should be capable of running on different OS platforms.
- Use any preferred automation framework (e.g., Selenium, Cypress).
- Choose a framework that supports the Page Object Model (POM) design pattern.
- Utilize test reporting tools (e.g., Extent Report, Allure report).
- Feel free to use any data provider (e.g., Excel, CSV).
- Use your imagination to write additional tests if they cover other important functionalities.

Remember, the more comprehensive, the better! 😏

## Task Submission

Feel free to put the code publicly on GitHub or a similar code control system.
```
Feel free to record a video of the test case execution and attach it as part of your solution. If you have any further questions or need assistance, feel free to ask! 🚀
```markdown
```