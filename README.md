## DOCKER APPLICATION DEPLOYMENT BY G23AI2067 (NEHA CHALLA):-

Basic Description:-

I (Neha Challa - G23AI2067) have created a Web application which Employee's Issue form where we can collect the basic details of employee like first name , last name,mobile number,email, martial status,Issue description and form will have submit button by pressing it form details will be collected this is the basic idea of it

Technologies used in this :-

1.  Angular 16.2.12 --- For creating the web application
2.  Angular Materials --- For styling the web applications
3.  Docker --- For creating the Docker images for the application we created 
4.  Git --- For pushing the code 

## Steps:- 

1. ## Create and Build Angular Application

   I have created Angular application namely Neha-assessment using this command

   ng new my-angular-app

   This will create the angular project where we can build the web application as required,After we make changes in the project we need to build the project by using this command

   ng build --configuration production

   which will create the dist folder and in this folder we will have production-ready files


2. ## Create a Docker File

   And now the web application is ready we need to create docker images for that we need to create a Docker file and this dockerfile needs to be present in the 
   project folder

3. ## Create Nginx Configuration file

    We need to create ngInx file in the root folder itself only, Creating an nginx.conf file is important for customizing the behavior of the Nginx server that will serve your 
    Angular application,In this file we will have port number, server_name

4. ## Build the Docker Image

    After this we need to run this coomand for building the docker images

    docker build -t neha-assessment .

   
5. ## Run Docker Container

   After the image is built, you can run it in docker container using the following commands

   docker run -d -p 80:80 my-angular-app

   
6. ## Access the application

    Open a web browser and navigate to http://localhost. You should see your Angular application running.


     And now i pushed this docker image into docker hub by using this both commands 

      docker tag neha-assessment neha200022/neha-assessment( For Tagging the image which needs to pushed into Docker Hub)
      docker push neha200022/neha-assessment (For Pushing it into the Docker Hub)

Now we need to test the Docker image which we created and pushed it into Docker Hub 

## Docker Image for checking purpose

The Docker image for this application is available on Docker Hub. You can pull and run the Docker image using the both commands:

docker pull neha200022/neha-assessment

docker run -d -p 80:80 neha200022/neha-assessment

After this try running the http://localhost and it should reflect like the same as below image



![image](https://github.com/user-attachments/assets/10dbf3e7-ff69-4298-8901-8259e914625f)


