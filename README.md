This is not working, unfortunately. I suggest creating it from scratch.



# EmptyBurpExtension
Getting IntelliJ to export the artifact (JAR) correctly is surpisingly difficult. This extension should assist with getting setup with IntelliJ.

1) Setup your project SDK (JDK)
2) Set you "src" folder as a source folder in File -> Project Structure -> Modules, then right click on "src" and click "Sources"
3) Add a new Artifact under  File -> Project Structure -> Artifacts. Create a Jar "From Modules with dependencies...". Set the main class to burp.BurpExtender.
4) Specify the output directory in File -> Project Structure -> Project Compiler Output. I would set the Project language level to 6, or else you may receive an "Invalid Source Release: 11" error. I'm not sure what causes this.
5) Need to unmark the root of the Module as excluded, but I can't do this for some reason.
