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


  #### Creating Docker Volume


  ![iScreen Shoter - 20250702143637862](https://github.com/user-attachments/assets/b5a44fc7-57b8-4171-8b57-1ab8392475e6)




  #### Deleting Volume 

  ![iScreen Shoter - 20250702145032312](https://github.com/user-attachments/assets/7e95fc49-e323-40a1-be9d-2659271848a5)
