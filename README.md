# How-to-run-gradle-on-termux
It will have 2 ways
Method 1: you need :
- source code link: for example thunderhack source code on github
-termux required
proceed :
Here I will take an example of https://github.com/CrystalCL/zeon-crack.git
1. Install Termux and install necessary tools:

Open Termux and install necessary packages like openjdk and gradle:

pkg update/
pkg upgrade/
pkg install openjdk-17 gradle
--------------------------------

2. Download source code from GitHub:

You need to download the source code from GitHub. Use the git command to clone the source code repository.

-pkg install git
-git clone https://github.com/CrystalCL/zeon-crack.git
cd zeon-crack
----------------------------------

3. Build with Gradle:

Before building, ensure that the build.gradle file has been configured properly to build the project.
You can now use Gradle to build the JAR file:

gradle build

If the build.gradle file has been configured correctly, this command will create a JAR file in the build/libs directory.
----------------------------------

4. Check results:

Once Gradle is complete, you can find the JAR file in the following directory:

ls build/libs

You will see the JAR file created there.

-----------------------------------
5. Run the JAR file (if necessary):

To run a JAR file, you can use the following command:

java -jar build/libs/<jar-file-name>.jar
