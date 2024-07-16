DOCKER APPLICATION DEPLOYMENT:-

Basic Description:-

I (Neha Challa - G23AI2067) have created a created a Web application which Employee's Issue form where we can collect the basic details of employee like first name , last name,mobile number,email, martial status,Issue description and form will have submit button by pressing it form details will be collected this is the basic idea of it

Technologies udes in this :-

Angular 16.2.12 --- For creating the web application
Angular Materials --- For styling the web applications
Docker --- For creating the Docker images for the We application we created 
Git --- For pushing the code 

Steps:- 

1. Create and Build Angular Application

   I have created Angular application using this command 

   ng new my-angular-app

   This will create the angular project where we can build the web application as required,After we make changes in the project we need to build the project by using this command

   ng build --configuration production

   which will create the dist folder and in this folder we will have production-ready files


3. Create a Docker File

   And now the web application is ready for this web application we need to docker images for that we need to create a Docker file and this dockerfile needs to be present in the 
   project folder

4. Create Nginx Configuration file

    We need to create ngInx file in the root folder itself only, Creating an nginx.conf file is important for customizing the behavior of the Nginx server that will serve your 
    Angular application,In this file we will have port number, server_name

5. Build the Docker Image

    After this we need to run this coomand for building the docker images

    docker build -t neha-assessment .

   
6. Run Docker Container

   After the image is built, you can run it in docker container using the following commands

   docker run -d -p 80:80 my-angular-app

   
8. Access the application







![image](https://github.com/user-attachments/assets/10dbf3e7-ff69-4298-8901-8259e914625f)


