1. Download Java SDK from this link http://www.oracle.com/technetwork/java/javase/downloads/jdk10-downloads-4416644.html
2. Install Java SDK
3. In the Environment Variables create new system variable with variable name "JAVA_HOME" and variable value c:\Program Files\Java\jdk-9.0.4\ (in your case value will be place where you install Java SDK)
4. Edit system variable "path" and add to this path variable name %JAVA_HOME%/bin;
5. Download Gradle and unpack
5.1. Download the latest Gradle distribution from this link https://gradle.org/next-steps/?version=4.9&format=all
5.2. Unpack the distribution
Create a new directory C:\Gradle with File Explorer.
Open a second File Explorer window and go to the directory where the Gradle distribution was downloaded. Double-click the ZIP archive to expose the content. Drag the content folder gradle-4.9 to your newly created C:\Gradle folder.
Alternatively you can unpack the Gradle distribution ZIP into C:\Gradle using an archiver tool of your choice.
5.3. Configure your system environment
In File Explorer right-click on the This PC (or Computer) icon, then click Properties -> Advanced System Settings -> Environmental Variables.
Under System Variables select Path, then click Edit. Add an entry for C:\Gradle\gradle-4.9\bin. Click OK to save.
5.4. Verify your installation
Open a Windows command prompt and run gradle -v to run gradle and display the version, e.g.:

$ gradle -v

------------------------------------------------------------
Gradle 4.9
------------------------------------------------------------
6. Clone repository to the local machine
7. Open a Windows command prompt from your place  where you clone repository (for example c:\annotation\) and run "gradlew test" (for example c:\annotation>gradlew test)
