Now we will download the Contrast Agent into your KataKoda instance. 

1. Create a directory for the Agent.

`mkdir /root/contrast`{{execute}}

2. Download the Contrast Agent into the directory you just created. 

`curl --fail --silent --location "https://repository.sonatype.org/service/local/artifact/maven/redirect?r=central-proxy&g=com.contrastsecurity&a=contrast-agent&v=LATEST" -o /root/contrast/contrast.jar`{{execute}}

3. Change the permissions on the Agent so that it can be executed at run-time. 

`chmod 755 /root/contrast/contrast.jar`{{execute}}

