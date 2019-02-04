# MavenAutomation

I have created a Maven Project and the POM.XML has the dependencies for Selenium Jars, TestNg , Extent Reports and Maven Sure Fire Plugins.

The Project has the following Structure

1) Src/Main/Java- These will have Page Objects and Utlity or Framework Classes which are resuable.
2) Src/Main/Resources- These will have resources used by SRC/Main/Java
3) Src/Test/Java- These will have the Test Scripts
4)Src/Test/Resources- These will have the Test related resources like property files

The Project flow is as below:

  1) we will trigger the test execution from TestNg XML with required parammeters like browser and other parameters by calling the corresponding test class
  2) Each test class extends Base Test which has the design to bringup the  HTML report and the design to determine the status of the test so as we take screenshot on failure
  3) The Utility Classes will give a driver instance, have the logic to read from property file and to take a screen shot.
  4) The Page Objects will have the logic to do the page operations which inturn extend the base class to reuse the framework level functions from BaseFunc class.
