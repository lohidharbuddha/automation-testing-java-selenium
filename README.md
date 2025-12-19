# automation-testing-java-selenium

Demo automation-testing repo using Java + Selenium + TestNG, with GitHub Actions CI.

What’s included
- Maven-based Java project
- TestNG tests using Selenium WebDriver
- WebDriverManager to automatically download browser drivers
- GitHub Actions CI workflow (runs on push/PR and nightly)
- Sample test that checks example.com page title

Quickstart
1. Clone:
   git clone https://github.com/lohidharbuddha/automation-testing-java-selenium
2. Build & run tests:
   mvn test

CI notes
- CI installs Chromium on the runner and uses WebDriverManager to manage chromedriver.
- Tests run headless by default (CI and local).

Project layout
- pom.xml
- src/test/java/... Example TestNG Selenium tests
- .github/workflows/ci.yml

Customize
- Switch to JUnit by replacing TestNG dependency and test classes.
- Add additional browsers by installing browser binaries in CI (Firefox, Edge).
- Add Codecov or coverage publishing if desired.
