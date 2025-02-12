# Bookswagon Automation Testing Project

## Overview
This project is an **end-to-end test automation framework** for the Bookswagon e-commerce platform, developed using **Selenium WebDriver with Java**. It follows industry best practices to ensure efficient and reliable test execution. The framework validates various user flows, enhances test maintainability using the **Page Object Model (POM)**, and generates detailed test reports.

## Key Features
- Automated end-to-end testing of the **Bookswagon** website.
- Implemented **Page Object Model (POM)** for better test structure and reusability.
- Functional and regression test cases for critical workflows.
- Test execution using **TestNG** with assertions and parameterization.
- Integrated **Extent Reports** for detailed test execution logs.
- Exception handling and **screenshot capturing** on test failures.
- Configurable **properties file** for URL, credentials, and test configurations.
- Parallel execution support for faster test runs.

## Technologies Used
- **Programming Language**: Java
- **Automation Framework**: Selenium WebDriver
- **Test Framework**: TestNG
- **Build Tool**: Maven
- **Reporting**: Extent Reports
- **Version Control**: Git, GitHub

## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/PromojitPaul/Bookswagon.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Bookswagon
   ```
3. Install dependencies using Maven:
   ```sh
   mvn clean install
   ```

## Running the Tests
- Execute all test cases:
  ```sh
  mvn test
  ```
- Run specific test classes using TestNG:
  ```sh
  mvn test -Dtest=LoginTest
  ```
- Generate **Extent Reports**:
  ```sh
  mvn test && mvn site
  ```

## Test Coverage
- **Login Functionality**: Valid and invalid login scenarios.
- **Search & Filter**: Searching for books and applying filters.
- **Cart & Checkout**: Adding/removing books and completing orders.
- **UI & Performance**: Ensuring responsiveness and smooth navigation.

## Folder Structure
```
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── base/             # Base class for test setup
│   │   │   ├── pages/            # Page Object Model (POM) classes
│   │   │   │   ├── LoginPage.java
│   │   │   │   ├── HomePage.java
│   │   │   │   ├── SearchPage.java
│   │   │   │   ├── CartPage.java
│   │   │   │   ├── CheckoutPage.java
│   │   │   ├── utils/            # Utility functions (Excel handling, config, etc.)
│   │   │   │   ├── ConfigReader.java
│   │   │   │   ├── ExcelUtils.java
│   │   │   │   ├── TestUtils.java
│   ├── test/
│   │   ├── java/
│   │   │   ├── tests/            # Test scripts
│   │   │   │   ├── LoginTest.java
│   │   │   │   ├── SearchTest.java
│   │   │   │   ├── CartTest.java
│   │   │   │   ├── CheckoutTest.java
│   │   │   ├── testdata/         # Test data files
│   ├── resources/
│   │   ├── config.properties     # Test configuration file
│   │   ├── testng.xml            # TestNG configuration
├── test-output/                  # Extent Reports and logs
├── reports/                      # Screenshots and logs from failed tests
├── pom.xml                        # Maven dependencies
├── README.md                      # Documentation
```

## CI/CD Integration
- Configured to run tests on **every code push**.
- Automated test execution using **GitHub Actions**.
- Generates test reports after execution.

## Conclusion
This **Selenium with Java** automation project demonstrates expertise in **test automation, framework design, and CI/CD integration**, making it an ideal addition to an SDET/QA portfolio.

## Contact
For more details, explore the repository or connect via GitHub.

