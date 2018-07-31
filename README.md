# Using SoapUI to Mock SOAP Services

The example in this directory is the Workday Human Resources WSDL.

It's been imported into SoapUI, a Mock Service created, and then this has been exported to a war, in the folder `workdaymocks`

To use it, perform the following:

* Add the war to tomcat & start tomcat
* view the webpage, http://localhost:8080/workdaymocks
* send traffic to http://localhost:8080/workdaymocks/workday-hr


Add the war to tomcat & start tomcat

```
# Set tomcat home
export TOMCAT_HOME=/usr/local/Cellar/tomcat/8.5.16_1/libexec/webapps
# Copy the exploded war to tomcat home
cp -rp workdaymocks ${TOMCAT_HOME}
# start tomcat
brew services start tomcat
```
