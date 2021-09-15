In this step we will create and configure the contrast_security.yaml file with the settings necessary in order for the Agent to communicate to the Team Server. 

1: Start by creating the initial contrast_security.yaml file. 

`cat << EOF > /root/contrast/contrast_security.yaml
api:
  url: https://ts.steve.contrast.pw/
  user_name:
  api_key:
  service_key:
application:
  name: WebGoat_Student##
  group: student##_group
agent:
  java:
    standalone_app_name: WebGoat_Student##
EOF `{{execute}}

2: Login to the Contrast Team Server using the credentials that were provided to you by the Instructor. You can navigate using a new tab in the browser or click the "Contrast URL" tab above the KataKoda terminal. 

https://ts.steve.contrast.pw/

3: Find the key elements you will need to populate In Organization Settings -> API. In the YAML file. You will need:  

1. Agent Username
2. Agent Service Key
3. API Key

4: Populate the contrast_security.yaml file with these values. You can use the KataKoda Editor in the top right portion of this screen to modify the file. 

1. Replace WebGoat_Student## with your student number for example if your student 10 your application name will be "WebGoat_Student10".
2. Also update the standalone_app_name field as this will ensure route coverage is applied to the java application.
