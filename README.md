# MavenAutomation

I have created a Maven Project with the POM.XML which has the dependencies for Selenium Jars, TestNg , Extent Reports and Maven Sure Fire Plugins.

The Project has the following Structure

1) Src/Main/Java- This will have the Page Objects and Utlity or Framework Classes which are reusable.
2) Src/Main/Resources- This will have resources used by SRC/Main/Java
3) Src/Test/Java- This will have the Test Scripts
4)Src/Test/Resources- This will have the Test related resources like property files

The Project flow is outlined below:

  1) I will trigger the test execution from TestNg XML with required parammeters like browser and other parameters by calling the corresponding test classes.
  2) Each test class extends Base Test which has the designs to bring up the  HTML report and the design to determine the status of the tests, so the system can take a screenshot upon failure.
  3) The Utility Classes will give a driver instance, have the logic to read from property file and to take a screen shot.
  4) The Page Objects will have the logic to do the page operations which in turn extend the base class to reuse the framework level functions from the BaseFunc class.
