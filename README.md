# SeleniumFramework

This test framework utilizes Selenium for browser automation and includes several other dependencies:
1. TestNG
2. Selenium API
3. Apache Commons
4. Extent Reports
5. Maven
6. Java
   
The framework is set up using the Page Object Model design pattern.
1. Each page of the application is represented by its own class (pages package).
2. The utils package contains the following classes:
   (a) ExtentReportHelper - used to create the extent report object (single object is created and it is used for multiple test scenarios.
   (b) ListenerHelper - uses ITestListener, which helps in creating the report as per different functions.
   (c) PropertyReaderHelper - helps to read the global cconfiguration file.
3. The base package is used and it includes the following classes:
   (a) SetupDriver – manages different drivers such as Chrome, Firefox, and Edge, triggered by the browserType key.
   (b) CustomWaits - simplifies the use of Thread.sleep into an easy-to-use function, applicable for both explicit and implicit waits.
   (c) Commons – sets up the JSON data file for test scenarios.
4. The TestConfiguration package includes BaseTest for setting up before and after test functions.
5. The TestData package manages the JSON file with test data.
6. TestNG features such as priority, description, dataProvider, and groups are all covered.
