## Task Manager Web Application

This is a simple task manager web application developed using HTML, CSS, and JavaScript and is hosted in a docker container.

## How to Run the Application Locally

To run the application locally, this repository could be cloned into your local machine or you could open the "index.html" file in your web browser.

## How to Build the Docker Image and Run a Container Using the Image
It is advisable to first have docker desktop installed on your machine.

# Steps
1. Navigate to the directory containing the Dockerfile and web application code,
2. Open your editor terminal,
3. Build the Docker image by running the following command: docker build -t your-docker-image-name (replace "your-docker-image-name" with the name you wish to call your docker image.
4. Once the image is built successfully, you can run a container using the image with the following command: docker run -d -p 8080:80 your-docker-image-name
This command starts a container called "your-docker-image-name". It maps port 8080 of the host machine to port 80 of the container.
5. Open your web browser and navigate to 'http://localhost:8080' to access the running web application.

## Assumptions or Decisions Made During the Development Process
1. I made sure that my web application is lightweight consisting only of HTML, CSS, and JavaScript all used in one index.html file to ensure ease of deployment and accessibility.
2. I used nginx as the web server to host my application and serve my static HTML file specifying a lightweight image called alpine as my linux distribution.
   
