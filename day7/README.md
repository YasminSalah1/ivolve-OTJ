# Day 7
## Lab 16: Docker Compose for Node.js + PostgreSQL App
- Clone source code and Dockerfile from https://github.com/ibrahim-Adel15/docker6.git
- Write a docker-compose.yml file that define the following:
  
  1. App as a service for node.js application
    - Builds the image from the provided Dockerfile in the cloned directory
    - Expose port 3000
    - Depends on the db service to ensure PostgreSQL is ready before the app starts
    - Use mynet network
  2. DB as a service for PostgreSQL Database
    - Uses the image: postgres:15-alpine
    - Runs on port 5432
    - Uses the following environment variables:
      - POSTGRES_USER: postgres
      - POSTGRES_PASSWORD: postgres
      - POSTGRES_DB: postgres
    -  Mounts a volume postgres_data for data persistence (/var/lib/postgresal/data)
    -  Use mynet network
  3. postgres_data as a volume
  4. mynet as a network



     #### - Docker Compose Build

     ![iScreen Shoter - 20250705005809271](https://github.com/user-attachments/assets/a9c8a0b5-2892-4561-991c-15be09e55baa)



     #### - App Running in Browser
  
     ![iScreen Shoter - 20250705005832977](https://github.com/user-attachments/assets/2683d454-6cb8-498c-a6ef-488fcd1b1596)




## Lab 17: Scan Docker Image with Trivy
- Install Trivy from https://trivy.dev/latest/getting-started/installation/
- Clone the Application Code https://github.com/Ibrahim-Adel15/Docker-1.git
- Write Dockerfile.
  - Use Maven base image
  - Copy the application code into the container
  - Build the app using mvn package
  - Expose port 8080
  - Run the jar file located in target/demo-0.0.1-SNAPSHOT.jar
- Build Image.
- Scan image and save the report in a JSON format.
- Push image into your DockerHub.


  #### Pushed Docker Image to DockerHub
  
  ![iScreen Shoter - 20250705021530068](https://github.com/user-attachments/assets/300895bf-8261-4c10-89e0-417c5d9d8119)


