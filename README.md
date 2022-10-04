
# Installations 
- INSTALL MAVEN
  - brew install maven
  - 
- UPDATE JAVA
  - brew install openjdk
  - sudo ln -sfn /opt/homebrew/opt/openjdk/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk.jdk
  - export JAVA_HOME="/Library/Java/JavaVirtualMachines/openjdk.jdk/Contents/Home"
  - java --version

# Source Code
- https://github.com/shazforiot/HelloWorld-Springboot-App

# Use Maven to create the WAR File 
- mvn clean package
- Maven will create a target folder, this folder will have the WAR

# Test the WAR locally
- java -jar <WAR_NAME>
  - Make sure the Java + JDK Version is correct (this might not work)

# Build Docker Image
 - docker build -t springboot:latest .

# Run Docker Image 
- docker run --name springbootapp -p 8080:8080 springboot