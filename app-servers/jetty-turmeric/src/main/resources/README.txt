This is a standalone web application server distribution for the Turmeric SOA project.
It includes all of the necessary runtime items.  Developers can use this installation
for testing of their turmeric soa services.  It can also be used as a basis for a
production deployment.

By default, the JPA providers will use Derby.  If you plan to use a different database
then you must add the appropriate JDBC jars.

RUNNING JETTY-TURMERIC:
=======================
To run with the default options:

  java -jar start.jar

To see the available options and the default arguments
provided by the start.ini file:

  java -jar start.jar --help

To run with add configuration file(s), eg SSL

  java -jar start.jar etc/jetty-ssl.xml

To run without the args from start.ini

  java -jar start.jar --ini OPTIONS=Server,websocket etc/jetty.xml etc/jetty-deploy.xml etc/jetty-ssl.xml

To run with JNDI support

  java -jar start.jar OPTIONS=Server,jsp

