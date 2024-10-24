# Build Instructions

1.) Open a virtual machine running Linux Ubuntu 22.04 (if this is not present on your machine, you can follow the guide here [TempLink](nothingyet))

2.) Check if terminal has git installed 
``` 
git version
git version 2.34.1
```
* If the expected output above does not match with your local machine install git, refer to instructions here: [Git Installation on Ubuntu](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

3.) Check if terminal has Java installed with a compatible version
```
java --version
openjdk 11.0.24 2024-07-16
OpenJDK Runtime Environment (build 11.0.24+8-post-Ubuntu-1ubuntu322.04)
OpenJDK 64-Bit Server VM (build 11.0.24+8-post-Ubuntu-1ubuntu322.04, mixed mode)
```
* If the expected output above does not match with your local machine install java, refer to instructions here: [Java Installation on Ubuntu](https://ubuntu.com/tutorials/install-jre#1-overview)

4.) Once the dependencies are installed, you can now clone the repository by executing the below commands. 
```
git clone https://github.com/MetroCS/cs3250_practice.git
```

5.) Install ant in order to be able to run the build targets defined in the build.xml file
```
sudo apt install ant
```

Verify ant installation using ant -version in the terminal, expected output should be 
```
Apache Ant(TM) version 1.10.12 compiled on January 17 1970
```


5.) Navigate to the ~/cs3250_practice/decision_support directory and run ant -p to see available build targets.

6.) To compile and build the executable, run the following command: 
```
ant main
```

7.) After running ant main the build files will be located in a new sub-directory "build", and the executable is available in the "jar" subdirectory beyond that.