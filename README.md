# thingslearned
Here i am going to capture all the links helped me.
<br>
Node:
http://stackoverflow.com/questions/22343224/whats-the-difference-between-tilde-and-caret-in-package-json
<br>
To find the actuall dependencies tree in the current project
npm ls >> tes.txt
<br>
Appache/Tomcat:
http://www.zeitoun.net/articles/client-certificate-x509-authentication-behind-reverse-proxy/start
<br>
scheduler:
https://gualtierotesta.wordpress.com/category/javaee/
<br>
lamda:
findFirst
skip(1)
<br>
WELD-001303: No active contexts for scope type javax.enterprise.context.RequestScoped
http://stackoverflow.com/questions/26631093/no-active-contexts-for-scope-type-javax-enterprise-context-requestscoped-when-in
or 
while running the test case,
add the @InRequestScope
<br>
Jersey:
http://howtodoinjava.com/jersey/jersey-custom-logging-request-and-response-entities-using-filter/
<br>
Hibernate:
@Enumerated(EnumType.STRING) ORA-01722 INVALID NUMBER = http://stackoverflow.com/questions/27979857/caused-by-java-sql-sqlsyntaxerrorexception-ora-01722-invalid-number-in-jpa-hi
<br>
http://stackoverflow.com/questions/19632805/jpa-java-lang-illegalargumentexception-not-an-entity
<br>
Maven:
http://stackoverflow.com/questions/6646959/difference-between-maven-scope-compile-and-provided-for-jar-packaging
<br>
By default, CDI beans are lazy loaded. It will invoke the postConstruct method while accessing the object.
<br>
http://geekabyte.blogspot.in/2013/09/fixing-converterhttpmessagenotwritablee.html
<br>
https://github.com/techwarriorz/Chat-App
<br>
https://connect2id.com/blog/importing-ca-root-cert-into-jvm-trust-store
<br>
#!/bin/bash
logfile=$1
if [ ! -f $logfile ]; then
  echo "log file not found $logfile"
  exit 1
fi
timestamp=`date +%Y%m%d`
newlogfile=$logfile.$timestamp
cp $logfile $newlogfile
cat /dev/null > $logfile
gzip -f -9 $newlogfile
<br>
