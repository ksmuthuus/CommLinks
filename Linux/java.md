# Java package

## Check version

```sh
java -version
```

## search available JDK versions

```sh
apt-cache search jdk
```

## Remove older version

```sh
yum remove java-1.7.*
```

## Install Java <http://openjdk.java.net/install/>

```sh
yum install java-1.8.*
```

## Set JAVA_HOME

```sh
find /usr/lib/jvm/java-1.8* | head -n 3
export JAVA_HOME =  /usr/lib/jvm/java-1.8.0-openjdk-1.8.0.242.b08-0.amzn2.0.1.x86_64
PATH=$PATH:$JAVA_HOME

#To Set it permanently
vi ~/.bash_profile
```
