## WAR file apache deploy

+ Extract war file from eclipse
     - [how to](https://www.codejava.net/ides/eclipse/eclipse-create-deployable-war-file-for-java-web-application)
     
---

+ local path check 
     - [how to](https://crunchify.com/how-to-start-stop-apache-tomcat-server-via-command-line-setup-as-windows-service/)
     - $catalina -h (local command)
     - check path 'Using CATALINA_BASE : /usr/local/Cellar/tomcat/9.0.7/libexec'
     - move WAR file to CATALINA_BASE 
    
---

+ Apache App Manager set
     - [how to](https://www.mkyong.com/tomcat/tomcat-default-administrator-password/)
     - go CATALINA_BASE/bin folder
     - Find out the process using command   ps -ef | grep tomcat
     - Start server: <Tomcat Root>/bin>./catalina.sh start
     - To Stop server: <Tomcat Root>/bin>./catalina.sh stop
     - localhost:8080 (browser)
     - appache app manager
     
---

+ Apache Tomcat User set
     - [how to](https://www.mkyong.com/tomcat/tomcat-default-administrator-password//)
     - add admin user info $TOMCAT_HOME/conf/tomcat-users.xml 
     
---
+ localhost:8080 (browser)
     - apache App Manager login
     - WAR file upload
     - uploaded WAR file deploy
     - localhost:8080/WAR file name

---
     
+ extra
     - Deploy to root directory
     - [reference](https://its-easy.tistory.com/4)
     
---

 
 