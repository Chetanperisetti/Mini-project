# Selenium Test Project

This project is a simple Selenium WebDriver automation test using **TestNG** that verifies the title and logo on the Amazon India website.

## Project Overview

This project automates basic tests on Amazon India's homepage using the Chrome browser. The tests include:

1. **Verifying the page title** to ensure it matches the expected value.
2. **Verifying the presence of the Amazon logo** on the homepage.

### Technologies Used
- **Java**: The primary language for writing the automation script.
- **Selenium WebDriver**: For browser automation.
- **TestNG**: For organizing and running the test cases.
- **ChromeDriver**: To interact with the Chrome browser.

## Prerequisites

Before running the project, ensure you have the following installed:

- Java Development Kit (JDK) 8 or later.
- [Eclipse IDE](https://www.eclipse.org/) or any other Java IDE.
- [Selenium WebDriver](https://www.selenium.dev/) library.
- [TestNG](https://testng.org/doc/) plugin for your IDE.
- [ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/) compatible with your Chrome browser version.

## Project Structure

The main class, `Program1.java`, contains three methods:
- **setUp()**: Initializes the WebDriver, opens the Amazon India website, and maximizes the browser window.
- **verifyTitle()**: Verifies that the page title matches the expected title of the Amazon homepage.
- **verifyLogo()**: Checks that the Amazon logo is displayed correctly on the homepage.
- **tearDown()**: Closes the browser session after the tests are completed.

## How to Run the Project

1. **Clone the Repository**:
   Clone the repository from GitHub (if you have uploaded it there) or download the project files.

   ```bash
   git clone [https://github.com/your-username/your-repository.git](https://github.com/Chetanperisetti/Mini-project.git)
   ```

2. **Set Up ChromeDriver**:
   Download and place the appropriate `chromedriver.exe` in your desired location. Update the `System.setProperty()` path in the `setUp()` method of the project to point to your local ChromeDriver.

   ```java
   System.setProperty("webdriver.chrome.driver", "path/to/chromedriver");
   ```

3. **Install Dependencies**:
   - Add the Selenium WebDriver JAR files to your project build path.
   - Ensure TestNG is configured in your IDE.

4. **Run the Tests**:
   - Run the test using TestNG by right-clicking the file and selecting **Run As** > **TestNG Test**.

## Test Cases

- **Test Case 1**: Verify the title of Amazon India's homepage.
  - Expected Result: The title should be "Online Shopping site in India: Shop Online for Mobiles, Books, Watches, Shoes and More - Amazon.in".
  
- **Test Case 2**: Verify the visibility of the Amazon logo.
  - Expected Result: The Amazon logo should be displayed on the homepage.

## After Test Execution

After each test method, the `tearDown()` method will be called to quit the browser.
