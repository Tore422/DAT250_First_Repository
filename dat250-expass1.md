Installed software
-------------------

Intellij Ultimate edition, version 2020.02<br>
Apache Maven, version 3.6.3<br>
Java Development Kit (JDK) version 14.0.2<br>
Git bash, version 2.28.0<br>

Installation progress report
-----------------------------

I already had the Git bash client installed, so I updated it by<br>
running the command "git update-git-for-windows"<br>
and verified by checking that the version was correct using the command "git version" in the Git Bash.

I had an earlier version of Intellij already installed, but since a new version had been released<br>
I had to download and follow the installation process anew from the jetbrains web site.<br>
After the installation was completed, I launched the IDE and configured a few of the settings.<br>
I then created a new project to confirm that it was indeed working.

I did not have Maven installed, so I downloaded and followed the instructions on https://maven.apache.org/install.html<br>
Verified that the installation was successful by using the command "mvn -v" in a command prompt,<br>
and comparing the output to what the Maven installation website showed.

I had a few JDKs already installed, but decided to install the latest version (14.0.2) in order to be up to date for this course.<br>
Verified by using the command "java -version" in a command prompt and confirming that the version displayed was correct.


Technical difficulties
-----------------------
After setting up Heroku and progressing through the<br>
getting started guide on https://devcenter.heroku.com/articles/getting-started-with-java#define-config-vars<br>
I ran into a problem with the command: heroku config:set ENERGY="20 GeV"<br>
Yielding the following error message: 'C:\Program' is not recognized as an internal or external command, operable program or batch file.
~~This problem is as of yet unresolved.~~<br>
Turns out the command would not accept the space between 20 and GeV, despite the guide insisting it should work.<br>
Heroku CLI now accepts the command, but a space is naturally missing between 20 and GeV on the web page.
