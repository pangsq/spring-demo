# gs-rest-service-complete demo

`complete` version of https://github.com/spring-guides/gs-rest-service.git

## used as tomcat app

```
mvn clean package war:war
# depoly the target/rest.war into /usr/local/tomcat/webapps/ or
# unzip the target/rest.war into /usr/local/tomcat/webapps/ROOT/

# run tomcat: /usr/local/tomcat/bin/catalina.sh run

# then access the url http://{tomcat_endpoint}/rest/greeting or http://{tomcat_endpoint}/greeting
```

## used as springboot jar

```
mvn clean package
java -jar target/rest.jar

# access the url http://127.0.0.1:8080/greeting
```

## deployed as a zip(with start.sh)

```
mvn clean package

# unzip target/rest-dist.zip -d <YOUR APP PATH>
```