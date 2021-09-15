You can now start your compiled WebGoat application with Contrast.

1: Let's start the Contrast Agent with the WebGoat Server.

`java -Dcontrast.config.path=/root/contrast/contrast_security.yaml -javaagent:/root/contrast/contrast.jar -jar /root/WebGoat/webgoat-server/target/webgoat-server-8.2.0.jar --server.port=8080 --server.address=[[HOST_IP]]`{{execute}}

2: Once your application is up and running you will need to browse to the application and exercise some of the routes. Note: if you don't stimulate the routes, the application will not successfully onboard into Contrast. 

http://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com/WebGoat

Or you can click on the WebGoat tab under the KataCoda Editor.
