Technical difficulties
-----------------------

After cloning the project from Git, Intellij would not run the project.<br>
Trying to build the project with maven failed, as the terminal of the IDE could not find the pom.xml file for some reason.<br>

It turns out that the problem was that the pom.xml file is located in the wrong directory...<br>
By moving the pom.xml from counters/counters/pom.xml to the top level (with the readme and .gitignore files)<br>
the project finally recognised the file.<br>
I then had to reload the maven dependencies (right click pom.xml --> maven --> reload project),<br>
mark the source and test root folders (might be an Intellij specific requirement),<br>
and then change some package names (which for some reason was also incorrect) in the other classes<br>
by appending main.java. to each package declaration, before the project would run.












Link to experiment code
------------------------



Experiment 2




(Experiment 3)




(Experiment 4)









Pending issues
---------------



None so far






