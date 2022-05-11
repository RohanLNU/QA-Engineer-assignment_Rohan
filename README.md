Project Setup & Implementation*****************************************************************************************************************************************

Framework developed using the design pattern as Page Object Model where I have created different packages for different functions.
Framework is made on the maven which is divided into two parts:-
1. SRC/MAIN/JAVA
2. SRC/TEST/JAVA

SRC/MAIN/JAVA:-
 
  1. com.assigment.action 
    - contains class (Action.java) which is having implementation of all the reusable methods from the ActionInterface. examples of the reusable methods are:- implicit wait, explicit wait, pageloadtimeout, action class, select class etc.
  2. com.assigment.actioninterface
   - contains Interface (ActionInterface.java) which is having the definition of the all the reusable methods.
  3. com.assigment.base
   - contains the (BaseClass.java) having the driverinitialization, browser setup, closing the driver.
  4. com.assigment.dataprovider
   - contains class (DataProviders.java) which is having implementation of all the dataproviders used for fetching the data from excel.
  5. com.assigment.pageObjects
   - It is having seperate class for the seperate pages & for each page there is method defined for performing action on the pages.
  6. com.assigment.utility
   - It contains (NewExcelLibrary.java) class for reaading & writing of the data from excel & then it is being called in the dataprovider class for fetching the data for each sheet.
  7. com.assigment.resource
   - It contains one sub-folder Test

SRC/TEST/JAVA:-

1. com.assigment.testcases
  - Having seperate test class with different test methods for seperate page object class using TestNG & also contains End-to-End test.


Project Execution******************************************************************************************************************************************************

- we are using the testng.xml file for running the test classes. I have created different testng.xml file naming testngall.xml which is containing the end-to-end testclass, testng_crossbrowser.xml file for cross browser testing & testng_regression.xml for regression suite test.

For running the file steps are:-
    1. import the project in your eclipse
    2. open the project in eclipse.
    3. scroll down -> right click any of the testng file. eg- testng_all.xml -> select run as TestNg Test.
    


  

