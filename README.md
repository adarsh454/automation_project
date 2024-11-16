
**In test > Java > part1:** there are two scripts:

1. For the FirstSeleniumTest script: 
This test script logs a user into https://opensource-demo.orangehrmlive.com/ and verifies, using assertions, whether the dashboard is displayed successfully.

2. For the LogInShouldFailTest script: 
This is a negative test for FirstSeleniumTest. Here, the test case annotated with @Test logs in to the URL and uses Assert.assertNotEquals to verify that the test should fail if the dashboard appears after login.


**In the directory test > Java > part2.com.saucedemo**, there are three scripts:

1. BaseTest:
Includes the @BeforeClass annotation, where it sets up the Chrome driver and navigates to the URL "https://www.saucedemo.com".
Also contains the @AfterClass annotation for the tearDown method.

2. LoginTest:
Contains a test case annotated with @Test, which sets an incorrect username and password.
Verifies the error message displayed on the UI using assertions.

3. ProductsTest:
Contains a test case annotated with @Test, which logs in to the application by calling a method from the LoginPage.
Uses a boolean method in LoginPage to assert whether the user is successfully logged in.






