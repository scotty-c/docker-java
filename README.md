#Java
scottyc/java

A simple Java container in CentOS 7.


##Running

Create a Dockerfile in your java project '''FROM''' scottyc/java
```
COPY . /usr/local/someapp
WORKDIR /usr/local/someapp
RUN javac App.java
CMD ["java", "App"] 
```
##Building
```
docker build -t someapp .
docker run --name app -d someapp
```