
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




Experiment repositories
------------------------

Experiment 1


Experiment 2




Database Inspection
-----------------------






Pending Issues
---------------




