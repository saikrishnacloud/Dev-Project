# My Java Web Application

A simple JSP web application packaged as a WAR file with Maven for deployment on Apache Tomcat.

## Requirements
- JDK installed
- Maven installed
- Apache Tomcat 9 (recommended for this Servlet 4.0 web.xml)

## Build
From this directory, run:

```bash
mvn clean package
```

The WAR file will be created at `target/myapp.war`.

## Deploy
Copy the WAR file into the Tomcat `webapps` directory, for example:

```bash
sudo cp target/myapp.war /opt/tomcat/webapps/
```

Start or restart Tomcat using the service name configured on your server. Then open:

`http://localhost:8080/myapp/`

For remote access, replace `localhost` with your server IP and ensure firewall/security-group rules allow the intended traffic on port 8080.
