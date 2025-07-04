# Day 6
## Lab 14: Docker Volume and Bind Mount with Nginx
- Create nginx_logs volume to persist Nginx logs and verify it in the default volumes path.
- Create a directory nginx-bind/html to serve a custom HTML file from your host machine.
- Create index.html file with "Hello from Bind Mount" syntax in nginx-bind/html directory.
- Run Nginx container with the following:
  - Volume for /var/log/nginx
  - Bind Mount for /usr/share/nginx/html
- Verify Nginx page by running curl command from your local machine.
- Change in the index.html file in your sal machine then verity Nginx page again.
- Verify logs is stored in the nginx logs volume.
- Delete the volume.


  #### - Creating Docker Volume


  ![iScreen Shoter - 20250702143637862](https://github.com/user-attachments/assets/b5a44fc7-57b8-4171-8b57-1ab8392475e6)




  #### - Deleting Volume 

  ![iScreen Shoter - 20250702145032312](https://github.com/user-attachments/assets/7e95fc49-e323-40a1-be9d-2659271848a5)





## Lab 15: Custom Docker Network for Microservices
- Clone the frontend and backend Code https://Rithub.com/Ibrahim-Adel15/Docker5.git
- Write Dockerfile for frontend and create image.
  - Use python image
  - Install packages in requirements.txt file
  - Expose port 5000
  - Run python command on app.py
- Write Dockerfile for backend and create image.
  - Use python image
  - Install flask
  - Expose port 5000
  - Run python command on app.py
- Create a new network called ivolve-network.
- Run backend container using ivolve-network.
- Run frontend container (frontend1) using ivolve-network.
- Run another frontend container (frontend2) using default network.
- Verify the communication between containers.
- Delete ivolve-network.


  #### - Container Communication within Custom Docker Network


  ![WhatsApp Image 2025-07-04 at 20 19 44](https://github.com/user-attachments/assets/9c066ac2-3014-45da-8485-b5d54d1330d6)


