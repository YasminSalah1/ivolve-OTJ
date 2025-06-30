# Day 5 
## Lab 11: Run Java Spring Boot App in a Container
- Clone the Application Code https://github.com/Ibrahim-Adel15/Docker-1.git
- Write Dockerfile.
  - Use Maven base image with java 17
  - Create work directory
  - Copy the application code into the container
  - Build the app using mvn package
  - Run the app on jar file located in target/demo-0.0.1-SNAPSHOT.jar
  - Expose port 8080
- Build Image.
- Run Container.
- Test the Application.
- Stop and delete the container.
- Repeat the steps, but build the application first before write Dockerfile.

  

  #### Container + Browser Output


  ![iScreen Shoter - 20250630175810218](https://github.com/user-attachments/assets/a175f98b-13e9-4fc2-bfd2-d7aaa2c97307)



## Lab 12: Multi-Stage Build for a Node.js App
- Clone the Application Code https://github.com/Ibrahim-Adel15/Docker-1.git
- Write Dockerfile with Multi-stage.
  - Use Maven base image for first stag
  - Copy the application code into the container
  - Build the app using mvn package
  - Use java base image for second stag
  - Copy JAR file from first stag
  - Expose port 8080
  - Run the app
- Build Docker Image.
- Run the container.
- Test the Application.
- Stop and delete the container.

  

  #### Container + Browser Output


  ![iScreen Shoter - 20250630192722124](https://github.com/user-attachments/assets/fee9543e-f12b-487a-874e-6416929b16de)

