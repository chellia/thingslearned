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

https://gist.github.com/danielestevez/2044589 git tag and upage
<br>
javascript, join(", ");

<br>
SSL in simple ->
https://www.ssl.com/article/ssl-tls-handshake-overview/
https://info.ssl.com/faq-what-is-a-private-key/
https://www.dynacont.net/documentation/linux/openssl/
https://www.digicert.com/blog/where-is-your-private-key/
https://wiki.apache.org/tomcat/tools/SSLTest.java
<br>
Apache proxy --
 1) To forward the ssl related headers to internal web application
  need to set this header
   RequestHeader set SSL_CLIENT_S_DN "%{SSL_CLIENT_S_DN}s"
 2) To read the certificate information from the internal application
    request.getHeader("ssl_client_s_dn")
 3) to read the proxy certificate
    certDN = certChain[0].getSubjectX500Principal().getName()
    extractAttributes
  <br>
  the java regex engine http://java-regex-tester.appspot.com/
  <br>
  know about private key https://info.ssl.com/faq-what-is-a-private-key/
  https://www.digitalocean.com/community/tutorials/openssl-essentials-working-with-ssl-certificates-private-keys-and-csrs
  <br>
  
  <br>
<br>
SSL / TLS
https://serverfault.com/questions/530430/create-a-public-private-key-pair-for-certificate-in-iis
https://www.digicert.com/ssl-support/pfx-import-export-iis-7.htm

https://support.accessdata.com/hc/en-us/articles/207830957-How-can-I-get-public-and-private-keys-out-of-IIS-

https://docs.druva.com/Knowledge_Base/inSync/How_To/Using_Microsoft_IIS_to_generate_CSR_and_Private_Key

https://www.devco.net/archives/2006/02/13/public_-_private_key_encryption_using_openssl.php
https://en.wikibooks.org/wiki/Cryptography/Generate_a_keypair_using_OpenSSL


https://docs.oracle.com/en/cloud/paas/database-dbaas-cloud/csdbi/generate-ssh-key-pair.html#GUID-69EF7E8A-7CD5-482E-A878-882EA21DE2B8
https://www.digitalocean.com/community/tutorials/openssl-essentials-working-with-ssl-certificates-private-keys-and-csrs

https://terry.im/wiki/terry/Use+OpenSSL+to+generate+key+pairs.html
<br>
  cipher suite details a: https://wiki.mozilla.org/Security/Server_Side_TLS#Recommended_configurations
   <br>
   
https://www.mulesoft.com/tcat/tomcat-ssl
<br>
Maven Resource
Resources plugin does the variable resolve. In assembly, we need to filtered to true.
<fileSet>
            <directory>assembly/version</directory>
            <outputDirectory>/</outputDirectory>
            <filtered>true</filtered>
        </fileSet>
<br>
https://stackoverflow.com/questions/40176003/cdiunit-test-with-junit-rule-is-impossible-because-of-a-public-private-field-pa

<br>
Annotation retention policy
RetentionPolicy.SOURCE: Won't appear in the decompiled class
RetentionPolicy.CLASS: Appear in the decompiled class, but can't be inspected at run-time with reflection with getAnnotations()
RetentionPolicy.RUNTIME: Appear in the decompiled class, and can be inspected at run-time with reflection with getAnnotations()
<br>
