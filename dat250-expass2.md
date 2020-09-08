
Technical problems
-------------------
While installing the Apache Derby database on windows,<br>
I found that setting the environment variables(EV) via the command line would not work,<br>
as the changes were reverted after closing the command line.<br>
To make the changes "stick", I had to manually update the EVs from windows properties (the system GUI).


While foolowing the vogella turtorial for experiment 1, I encoutered a few problems.<br>
1. In EclipseLink version 2.7.7, the file "javax.persistence_*.jar"<br>
   had been changed to "jakarta.persistence_2.2.3.jar", inititally making it difficult to locate.
2. When trying to run the test application in step 4, the program could not find the embedded drivers for derby.<br>
   With some help from my project team members, the problem got resolved by adding the <br>
   derby lib folder, from the derby installation path, to the list of project dependencies.
3. The class JpaTest from the turtorial had a bug in the deletePerson test,<br>
   resulting in most of the tests not functioning as intended.<br>
   The test was set to delete a person from the database with a last name ending<br>
   in an exclamation mark and not the number 1 as it should have.<br>
   Since the test was expecting an exception for not finding the user after it got deleted,<br>
   it was easy to miss that it did not find the user to be deleted in the first place...<br>
   Fixing this bug required modifying parts of the class, such as:
   * Using a try/catch looking for the exception only on the part checking for the deleted person.<br>
   * Adding code for removing the family connection to the deleted person.
   * Adding code for re-adding the person to the database after deletion.
   * (for convenience) Added a family to the persons being created in setUp() and deletePerson().
   




Experiment repositories
------------------------

Experiment 1<br>
https://github.com/Tore422/DAT250_JPA_Assignment_Experiment1_Simple
https://github.com/Tore422/DAT250_JPA_Assignment_Experiment1_Eclipselink


Experiment 2<br>
https://github.com/Tore422/DAT250_JPA_Assignment_Experiment2



Database Inspection
-----------------------

I used the ij scripting tool for inspecting the database,<br>
after having added data by running the application a couple times.




![inspecting database for experiment 2, showing table contents](https://github.com/Tore422/DAT250_First_Repository/blob/master/JPA_Experiment2_checking_the_database.png)

![inspecting database for experiment 2, showing tables](https://github.com/Tore422/DAT250_First_Repository/blob/master/JPA_Experiment2_checking_the_database_tables.png)


The pictures show the code I used to inspect the database, if more information is needed just ask.

Pending Issues
---------------

None


