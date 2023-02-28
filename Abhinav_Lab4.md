# Lab Report 4

**Step 4**

ssh cs15lwi23adw@ieng6.ucsd.edu`<enter>`
![step4](ssh.png)

The single command used here is to log into the remote desktop. You then have to press `<enter>` to make the command actually run.


**Step 5**

git clone git@github.com:abhinavsanisetty/lab7.git`<enter>`
cd lab7`<enter>`

![step5](failTest.png)

The first command is used to clone the reporsitory that I forked to my github account in the setup. The link used is an ssh link instead of the standard HTTPS link. The ssh link is used instead because that way you dont need to login to your account again. The second command is used to switch into the lab7 directory so that I can run the JUnit tests in the next step. I pressed `<enter>` after each command to make the command actually run.

**Step 6**

javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar \*.java`<enter>`
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples`<enter>`


