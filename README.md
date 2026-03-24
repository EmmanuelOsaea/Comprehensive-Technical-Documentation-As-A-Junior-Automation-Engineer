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
# * Java JDK installed
# * Maven or Gradle for dependency management(Gradle example here)
# * Appium server installed and running
# * Android Emulator or real device connected
# * Android Finance tracker app

# 2. Maven pom.xml Dependencies (for Java + Appium)
<project xmlns = " " ...>
<modelVersion>    </modelVersion>
<groupId> </groupId>
<artifactId>appium-demo</artifactId>
<version> </version>

<dependencies> 
<!-- Appium Java client -->
<dependency>
<groupId>io.appium</groupId>
<artifactId>java-client</artifactId>
<version> </version>
</dependency>

<!-- Selenium WebDriver (Appium depends on it) -->
<dependency>
<groupId> </groupId>
<artifactId> </artifactId>
<version> </version>
</dependency>
  
<!-- TestNG for test framework -->
<dependency>
<groupId>org.testng</groupId>
<artifactId>testng</artifactId>
<version> </version>
<scope>test</scope> 
</dependency>
</dependencies>
</project>


.

# 3. Java + Appium Test Script Example




# 4. Explanation of the Example
# Java Concept Demonstrated: 

