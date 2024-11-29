**Running Liferay Quarterly releases on Wildfly 26.1.0**

WildFly is a lightweight version of JBoss

<https://www.wildfly.org/>

1. Download the necessary files for Liferay:\
   <https://customer.liferay.com/en/downloads>

   1. DXP WAR

   2. OSGI Dependencies

2. Check the README in wildfly/standalone/deployments/ROOT.war

3. Check the README in osgi

4. Check and set portal-ext.properties.\
   You need to set the database connection, because it will not run with hsql.

5. To start the bundle:

   1. Switch to Java 8

   2. Linux and Mac:\
      wildfly/bin/standalone.sh

   3. Windows:\
      wildfly/bin/standalone.bat

Patching-tool is configured so you can install patches the same way you do on tomcat.
