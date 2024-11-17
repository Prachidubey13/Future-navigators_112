# SauceDemo E-Commerce Testing Project

## Overview
This project implements automated testing for the SauceDemo e-commerce platform using Selenium WebDriver, Java, and the Page Object Model (POM) design pattern. It provides comprehensive end-to-end testing of critical user journeys, including user authentication, shopping cart management, and the checkout process.

## Features Tested
### User Authentication
- Login functionality
- Error handling for incorrect login
- Logout functionality

### E-commerce Functionality
- Product selection and addition to cart
- Cart management
- Product sorting (ascending and descending)

### Checkout Process
- Filling checkout form
- Completing the order
- Success message verification

## Technologies Used
- Selenium WebDriver (Java)
- TestNG for test execution
- Page Object Model (POM) for maintainability
- Maven for project management and dependency handling
- Java for test automation
- SauceDemo website as testing environment

## Project Structure
bash
```
src/
 ├── main/
 │   ├── java/
 │   │   ├── Pages/
 │   │   │   ├── CartPage.java           # Cart-related actions
 │   │   │   ├── CheckoutPage.java       # Checkout process actions
 │   │   │   ├── HomePage.java           # Homepage actions
 │   │   │   ├── LoginPage.java          # Login functionality
 │   │   ├── utils/
 │   │   │   ├── ConfigReader.java       # Reads data from the config file
 ├── test/
 │   ├── java/
 │   │   ├── Test/
 │   │   │   ├── SauceDemoTest.java      # Test cases for SauceDemo application
 ├── resources/
 ├── test-output/                        # TestNG output folder
 ├── config.properties                   # Configuration properties file
 ├── extent.html                         # Extent Report
 ├── pom.xml                             # Maven dependencies and build file
```

## Setup and Running Tests

### Prerequisites
- Java 11 or higher
- Maven (for dependency management)
- Selenium WebDriver
- TestNG (for test execution)

### Installation
1. Clone the repository:
bash
git clone https:


2. Navigate to the project directory:
bash
cd SauceDemo-Automation-Project


3. Install dependencies:
bash
mvn install


### Running Tests
Headless mode:
bash
mvn clean test -Dtest=SauceDemoTest


Test Runner (Interactive mode with reports):
bash
mvn test


## Best Practices Implemented
- Page Object Model for improved maintainability
- Explicit wait strategies using WebDriverWait
- Descriptive test and method naming
- Reusable methods for common actions (e.g., login, add to cart)
- Comprehensive error handling and verification
- Extent Reports for detailed test results and logs

## Future Enhancements
- Add API testing layer
- Implement data-driven testing
- Add visual regression tests
- Integrate with CI/CD pipeline

## Contributing
1. Fork the repository
2. Create your feature branch:
bash
git checkout -b feature/AmazingFeature

3. Commit your changes:
bash
git commit -m 'Add some AmazingFeature'

4. Push to the branch:
bash
git push origin feature/AmazingFeature

5. Open a pull request

## Notes
- This project uses the SauceDemo demo site for testing purposes.
- Test data is currently hardcoded; consider using external test data for scalability.
- Some tests may need adjustments based on the demo site's state.

## Author
Prachi dubey
