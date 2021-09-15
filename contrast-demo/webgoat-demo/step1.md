Welcome to our first lab exercise. In the bottom right portion of your web browser, you should see a Linux terminal. This is where we will run our commands in order to build WebGoat and instrument the Contrast Agent.

You'll also note that at the top of the terminal window, you should see "Terminal", "Contrast UI", and "WebGoat". Clicking on these tabs will either bring you back to the temrinal window, open the Contrast Team Server URL, or connect you to your WebGoat instance once you build and run it. Above the terminal, you'll see the file system. You can navigate between folders using the directory structure.  

Step 1: Clone the most recent WebGoat repository into your KataKoda Linux instance.

`git clone https://github.com/WebGoat/WebGoat.git`{{execute}}

Step 2: Build the Webgoat application from source using Maven. 

`cd WebGoat`{{execute}}

`mvn clean install -DskipTests`{{execute}}

You can open a new terminal tab and continue with the lab while the application compiles
