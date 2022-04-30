# Introduction to Java REST API

## Requirement

1. Server REST API
2. Client consume API

## Prerequisite

### Git

- Download [Git for Windows Setup](https://git-scm.com/download/win) - 64-bit Git for Windows Setup.

### Java & Maven

- Download file [OpenJDK8U-jdk_x64_windows_hotspot_8uxxx.zip](https://github.com/adoptium/temurin8-binaries/releases/) and extract to path `C:\Dev\Java\jdk8`
- Download file [apache-maven-3.8.x-bin.zip](https://maven.apache.org/download.cgi) and extract to path `C:\Dev\Java\apache-maven-3.8.x`
- Add java and mvn command to `$PATH` at `~/.bashrc`

```sh
### Java and Maven ###
export JAVA_HOME=/c/Dev/Java/jdk8
export MAVEN_HOME=/c/Dev/Java/apache-maven-3.8.5
export PATH=$JAVA_HOME/bin:$MAVEN_HOME/bin:$PATH

### ALIAS ###
alias mvn='mvn -Djava.net.useSystemProxies=true -Dmaven.wagon.http.ssl.insecure=true'
```


## 1. Server REST API

### Step 1. Create Project

- goto https://start.spring.io/
- create server-rest-api

### Step 2. Run

```
cd server-rest-api
./mvnw clean spring-boot:run
```

open:

- http://localhost:8080/
- http://localhost:8080/h2-console

### Step 3. Develop

- https://spring.io/guides/tutorials/rest/

### Step 4. Test

### Step 5. Package

```
./mvnw clean package -DskipTests
java -jar target/*.jar
```

## 2. Client consume API

### Step 1. Create Project

### Step 2. Run

### Step 3. Develop

### Step 4. Test

### Step 5. Package