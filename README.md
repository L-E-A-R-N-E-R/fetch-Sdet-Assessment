# fetch-Sdet-Assessment

### Link to the problem statement: https://fetch-hiring.s3.amazonaws.com/SDET/Fetch_Coding_Exercise_SDET.pdf

My project folder size was larger than 25MB due to which, I could not upload it on GitHub. You can download the project zip file from the below link. Apologies for any inconvenience caused.

https://drive.google.com/file/d/1JixUyfg1qw_XlGCkBEw76i7D1q_Vsv_k/view?usp=drive_link

Note: In case you want to save time, or are unable to run the project due to some build issues, here is a short video where I demonstrate the entire project in a screen recording.

https://drive.google.com/file/d/1T4ltkFgAbdbNV78R9f-mcFtu1MpNyTiy/view?usp=sharing

For simplicity, the driver used for automation is Chrome. 

# This project requires the following tools to run properly in any system

1. JDK 11
2. Docker Desktop

# In case you don’t have JDK 11 installed, kindly refer to these short clips

1. For Windows: https://www.youtube.com/watch?v=23FrsQiCBhA

2. For Mac

To download jdk: https://www.youtube.com/watch?v=bUKuKhywaiI&t=14s

Then follow these commands

![image](https://github.com/L-E-A-R-N-E-R/fetch-Sdet-Assessment/assets/41851792/c4d4e3de-386c-4fb2-8132-9af58dee737e)

If you still need help, please watch the full video: https://www.youtube.com/watch?v=oiqKK0FOjK0

3. Lastly, in order to confirm the successful setup of JDK 11 in your machine, execute the following commands

java -version

# In case you don’t have Docker Desktop installed, here are the links to the official documentation

For Windows: https://docs.docker.com/desktop/install/windows-install/

For Mac: https://docs.docker.com/desktop/install/mac-install/

# To run the program

## 1. For Windows user

1. Open the Docker desktop and make sure the Docker engine is running (The status is shown on the bottom left part of the screen)

![image](https://github.com/L-E-A-R-N-E-R/fetch-Sdet-Assessment/assets/41851792/ebbd7265-1d87-4728-9560-ffb32b7dfd53)

2. Open the terminal and execute the command

   *docker pull selenium/standalone-chrome*

   This might take a minute or two, depending on your internet connection. This command will pull the required selenium image from the docker hub.

3. Then execute the command

   *docker run -d -p 4444:4444 -p 7900:7900 --shm-size="2g" selenium/standalone-chrome:latest*

    This command will run the container. Let it run in the background since we need this container to be up and running for our main Selenium script to execute and show correct results.

4. Download the project zip file from the Google Drive link.

5. Open another terminal and navigate to the working directory of the project called GoldBar

   cd GoldBar

6. Execute this command in your terminal to compile your Java program
	
	"javac -cp lib\\* src\App.java"

	Note: Make sure you are in the GoldBar directory when you execute this command

7. Execute this command in your terminal to run your Java program

	"java -cp “src;lib\\*” App"

8. After a few seconds, you should see the following output on your screen

![image](https://github.com/L-E-A-R-N-E-R/fetch-Sdet-Assessment/assets/41851792/8689ee84-90d0-48ef-91d6-98dcbd7f4fd7)

Note: In order to witness the full automation on the http://sdetchallenge.fetch.com/ website in action, visit the link http://localhost:7900/?autoconnect=1&resize=scale&password=secret quickly after executing the java command in step 7.

# For Mac user

1. Open the Docker desktop and make sure the Docker engine is running (The status is shown on the bottom left part of the screen)

![image](https://github.com/L-E-A-R-N-E-R/fetch-Sdet-Assessment/assets/41851792/ebbd7265-1d87-4728-9560-ffb32b7dfd53)

2. Open the terminal and execute the command

*$ docker run --rm -it -p 4444:4444 -p 5900:5900 -p 7900:7900 --shm-size 2g seleniarm/standalone-chromium:latest*

Note: Mac users may have different architectures for which the docker run command can differ. Please refer to the below link for further assistance

https://github.com/SeleniumHQ/docker-selenium#experimental-mult-arch-aarch64armhfamd64-images

3. Download the project zip file from Google Drive link.

4. Open another terminal and navigate to the working directory of the project called GoldBar

   cd GoldBar

5. Execute this command in your terminal to compile your Java program

	javac -cp "lib/*" src/App.java

  Note: Make sure you are in the GoldBar directory when you execute this command

6. Execute this command in your terminal to run your Java program

	java -cp “src:lib/*” App

7. After a few seconds, you should see the following output on your screen

 ![image](https://github.com/L-E-A-R-N-E-R/fetch-Sdet-Assessment/assets/41851792/86bb320a-d294-4bce-ab29-4b29dfd19a9b)

Note: In order to witness the full automation on the http://sdetchallenge.fetch.com/ website in action, visit the link http://localhost:7900/?autoconnect=1&resize=scale&password=secret quickly after executing the java command in step 6.

