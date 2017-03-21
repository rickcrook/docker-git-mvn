# docker-git-mvn
dockerfile for docker, git, java and maven
Built for use as an image in gitlab-ci
Merge from:
   + https://github.com/carlossg/docker-maven
   + https://github.com/docker-library/docker

## Build
```
$docker build -t docker-git-mvn .
```

## Versions
```
$ docker run -it --rm --name docker-git-mvn docker-git-mvn java -version
openjdk version "1.8.0_121"
OpenJDK Runtime Environment (IcedTea 3.3.0) (Alpine 8.121.13-r0)
OpenJDK 64-Bit Server VM (build 25.121-b13, mixed mode)

$ docker run -it --rm --name docker-git-mvn docker-git-mvn mvn -version
Apache Maven 3.3.9 (bb52d8502b132ec0a5a3f4c09453c07478323dc5; 2015-11-10T16:41:47+00:00)
Maven home: /usr/share/maven
Java version: 1.8.0_121, vendor: Oracle Corporation
Java home: /usr/lib/jvm/java-1.8-openjdk/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "linux", version: "4.9.12-moby", arch: "amd64", family: "unix"

$docker run -it --rm --name docker-git-mvn docker-git-mvn git --version
git version 2.11.1

$docker run -it --rm --name docker-git-mvn docker-git-mvn docker --version
Docker version 17.03.0-ce, build 60ccb22
```
