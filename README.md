# Rediff Account Registration Automation Project

This is a **Maven‑based Selenium automation project** developed using **Java and TestNG**.  
The project automates the **Rediff Create New Account** page and covers dropdown handling, form validation, and basic framework design.

---

## Project Objective

The main objective of this project is to:
- Automate a real web application
- Handle dropdowns and dynamic elements
- Validate form inputs and selected values
- Follow Page Object Model (POM)
- Generate TestNG execution reports

---

## Application Details

- **Application Name:** Rediff Mail
- **URL:** https://mail.rediff.com/cgi-bin/login.cgi
- **Feature Automated:** Create New Account page

---

## Automation Flow

The following steps are automated in this project:

1. Launch the browser (Chrome / Edge)
2. Open Rediff login page
3. Validate landing page URL and title
4. Click on **Create New Account**
5. Enter user name and email
6. Handle auto‑suggested email options
7. Enter password
8. Select **Alternate ID checkbox**
9. Select Date of Birth using dropdowns
10. Fetch all country values from Country dropdown
11. Print total country count
12. Select country **India**
13. Validate selected country
14. Select city from dropdown
15. Capture screenshots on failure
16. Capture final execution screenshot
17. Close the browser

---

## Technologies Used

- **Programming Language:** Java
- **Automation Tool:** Selenium WebDriver
- **Test Framework:** TestNG
- **Build Tool:** Maven
- **Design Pattern:** Page Object Model (POM)
- **Reporting:** TestNG Default HTML Report
- **Version Control:** Git

---

## Project Structure

```
dropdown-menu-handling
│
├── src
│   ├── main
│   │   ├── java
│   │   │   ├── browser        # Browser setup and driver initialization
│   │   │   ├── config         # Configuration reader classes
│   │   │   ├── pages          # Page Object Model classes
│   │   │   └── utils          # Utility classes (Screenshot, ElementUtils, etc.)
│   │   └── resources          # Application resource files
│   │
│   └── test
│       ├── java
│       │   └── tests          # TestNG test classes
│       └── resources          # Test-specific resources
│
├── Object Repository
│   └── object.properties     # Test data and configuration values
│
├── screenshots
│   └── Final_Execution_State.png  # Screenshots captured during execution
│
├── target                    # Maven generated files
├── test-output               # TestNG generated reports
│
├── pom.xml                   # Maven project configuration
└── testng.xml                # TestNG execution configuration
```
---

### Package Description

- **browser** – Handles browser initialization (Chrome, Edge)
- **config** – Reads values from the properties file
- **pages** – Contains Page Object classes for UI actions
- **utils** – Contains reusable utility methods (screenshots, element checks)
- **tests** – Contains TestNG test cases
- **Object Repository** – Stores external test data and configuration
- **screenshots** – Stores screenshots for failures and final execution
- **target** – Maven build output folder
- **test-output** – TestNG HTML reports

---

## Framework Highlights

- Page Object Model for clean design
- Reusable methods for better maintenance
- Explicit waits for synchronization
- Hard and Soft Assertions for validation
- Screenshot capture on test failure
- Final screenshot after successful execution
- Browser selection using TestNG parameters
- Maven for dependency management

---

## Dropdown Handling

Dropdowns are handled using Selenium's **Select** class.
- All values are fetched and printed
- Total count is displayed
- Specific value (**India**) is selected
- Selected value is validated

---

## Screenshot Handling

- Screenshots are captured when assertions fail
- Screenshots help in debugging failures
- A final screenshot is captured after full automation run
- Screenshots are stored in the `screenshots` folder

---

## Reporting

- TestNG default HTML reports are generated automatically
- Important steps are logged using `Reporter.log()`
- Reports show test status, logs, and failure details

---

## How to Run the Project

### Using Maven
mvn test
### Using IDE
- Open the project
- Run `testng.xml` file

---

## Browser Configuration

Browser can be changed using TestNG parameters:
- Chrome
- Edge

Default browser is Chrome.

---

## Conclusion

This project demonstrates a **basic yet real‑time Selenium automation framework** following industry practices.  
It is suitable for learning Selenium automation, TestNG concepts, and Maven project structure.
