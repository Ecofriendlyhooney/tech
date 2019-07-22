# GCP & Domain Link
---

### Source backup 
+ Commit source code to Github repository

### Create Bitnami VM instance
+ DNS 1,2,3,4 check(copy)
    
### Godaddy.com(Domain Registered Site) DNS setting
+ DNS 1,2,3,4 set(paste)

### Build source code from Local environment
+ export project as name of 'ROOT.war'
     - with source (include source files so that can amend Cli directly afterwards) 

### Create GCP Cloud SQL for MySQL
+ create database
+ create table
+ copy Public IP address (and set to(*1))
+ CONNECTION Authorised networks (+Add Network with Bitnami instance's External IP)
+ USERS
      - Create user 

### WAR file upload to Bitnami VM instance
+ uplode Local's 'ROOT.war' to Bitnami vm instance /opt/bitnami/apache-tomcat/webapps
+ rename ROOT folder 
+ /opt/bitnami/apache-tomcat/conf
    - tomcat-users.xml (user auth add)
+ /opt/bitnami/apache-tomcat/webapps
    - ROOT folder files check    
+ /opt/bitnami/apache-tomcat/webapps/ROOT
    - index.* (edit as like)
+ /opt/bitnami/apache-tomcat/webapps/ROOT/WEB-INF
    - spring-servlet.xml 
    - ex)  <property name="url" value="jdbc:mysql://SQL instance URL/Database Name"
    - ex)  <property name="url" value="jdbc:mysql://33.203.80.232/spring" (*1)
+ /opt/bitnami/apache-tomcat/conf    
    - web.xml (edit <welcome-file-list>)
+ /opt/bitnami/apache-tomcat/bin
    - ./catalina.sh stop (server stop - Linux )
    - ./catalina.sh start (server start - Linuxpw) 
    
### Connect