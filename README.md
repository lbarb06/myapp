Build a Docker image containing a Node.js application and deploy it.

Pre-requisites:
- Node.js
- Docker Desktop
- Docker

1. Create the required files:
   - Dockerfile
     - chmod 644 Dockerfile
   - myapp-deployment.yaml
   - myapp-service.yml
   - package.json
   - server.js
     
3. Build the Docker image and list:
   
   `% docker build -t myapp:1.0 .`

   `% docker images`

4. Run the container to launch server.js and list the image:

   `$ docker run -d -p 3000:3000 myapp:1.0`

   `% docker images`

3. Test it by loading http://localhost:3000 on your browser to view text from res.send()

   `Hello from Docker!`

5. Stop the container and remove it

   `docker stop <CONTAINER ID>`

   `docker rm <CONTAINER ID>`

6. Remove the image

   `docker rmi <IMAGE ID>`
