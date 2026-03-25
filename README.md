# Practice Problems for You to Solve(Opera Ai)
# Problem 1: Locator Not Found
Your test fails with an error "NoSuchElementException" when trying to find a login button. The webpage was updated, and the button's ID changed from loginBtn to loginButton. How do you fix this?

# Problem 2: Test Timeout
Your test waits for a page element to appear but times out after 10 seconds. The element sometimes takes longer to load. How can you improve your test to handle this?

# Problem 3: API Test Unauthorized
Your API test for user registration returns a 403 Forbidden error. The API key might be invalid. What steps do you take to debug and fix this?

# Problem 4: Flaky Test in CI
A test passes on your local machine but fails randomly in the CI pipeline. What are possible causes and how do you investigate?

# Problem 5: Script Throws Exception
Your test script throws a NullPointerException when trying to access a web element. What could be the cause and how do you resolve it?


# Solution 1: Locator Not Found
Locate the button id test script and change it from loginBtn to LoginBtn
# Solution 2: Test Timeout
Research on how it can stay stable and prevent it from loading further than needed.
# Solution 3: API Test Unauthorized
Research on what often causes "403 forbidden error" then identify it inorder to solve it quickly. 
# Solution 4: Flaky Test in CI
Research on what causes test to pass on my local machine but fail in my ci pipeline and make corrections needed. 
# Solution 5: Script Throws Exception
Research on what "NullPointerException" means then identify what causes it to appear when attempting to access a web element.

# Practical Example: Java + Appium Basic Mobile Automation Test
# 1. Prerequisites
 #    • Java JDK installed
 #    • Maven or Gradle for dependency management(Gradle example here)
 #    • Appium server installed and running
   #  • Android Emulator or real device connected
   #  • Android Demo Quiz app

# 2. Gradle Dependencies (for Java + Appium)
```// build.gradle (Groovy DSL)
plugins {
id 'java'
}

group = 'com.example'
version = '1.0-SNAPSHOT'

repositories {
mavenCentral()
}

dependencies {
// Appium Java client
implementation 'io.appium:java-client: 10.1.0'
// Selenium WebDriver
implementation org.seleniumhq.selenium.selenium-java:4.41.0

// Testng for test Framework
testImplementation 'org.testng:testng: 7.12.0'
}

test {
useTestNG()
}
```
# 3. Java + Appium Test Script Example
```
import io.appium.java_client.android.AndroidDriver;
import io.appium.java_client.android.options.UiAutomator2Options;
import org.openqa.selenium.By;
import org.testng.Assert;
import org.testng.annotations.*;
import java.net.URL;
import java.time.Durations;

public class QuizAppTest {
   private AndroidDriver driver;

@BeforeMethod
public void setUp() throws Exception {
// Use UiAutomator 2Options for modern Appium 2.x
UiAutomator 2Options optiom = new UiAutomator2Options;

.setPlatformName("Android")
.setDeviceName("Emulator")
.setApp("path/to/app.apk")
.setAutomationName("UiAutomator2")

// Standard 4723 port
driver = new AndroidDriver (new URL("http 127.0.0.1.4723"),options);
driver.manage().timeouts().implicitlyWait(Duration.OfSeconds(7));



@Test
public void testQuizFlow(){
// Example flow: Start -> Answer -> Verify
driver.findElement(By.id("com.example.quiz.idbtn_start")).click()
driver.findElement(By.id("com.example.quiz.idoption_b")).click()
driver.findElement(By.id("com.example.quiz.idbtn_submit")).click()
Assert.assertTrue(driver.findElement(By.id("com.example.quiz.id/tv_submit")).isDisplayed());
}

@AfterMethod

public void tearDown() {
if (driver != null) driver.quit();
}
}
```

# 4. Explanation of the Example
# Java Concept Demonstrated: 
Class definition (QuizAppTest)
Methods with annotations (@BeforeMethod, @Test, @AfterMethod) from TestNg
Object Instantiation (Android Driver)
Variables and method Calls 
Assertions to verify results

# 5. Testing Types I Recommended for The Demo App I Built Using Ai from Scratch
 # Functional Testing 
   Submit Button records scores✓
# Regression Testing
   Adding the timer did not break the score✓
# Smoke testing
   App Opens✓


# App link below

https://github.com/EmmanuelOsaea/Quiz-app-Front-end-Web-design-
