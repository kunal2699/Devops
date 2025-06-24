# Devops

  - Download the github repo
  - Run the docker Command:
     Docker-compose up --build

# How the Rounting works
- In the assignment, routing is managed by Nginx, which acts as a reverse proxy to direct incoming HTTP requests to the appropriate backend services (service1 and service2)
- Nginx as a Reverse Proxy: Nginx listens for incoming HTTP requests on a specified port (in this case, port 8080). Based on the request path, it determines which backend service should handle the request.
- Service Endpoints: Each service has its own set of endpoints (routes) that are defined in the application code. For example:
service1 has endpoints /service1/ping and /service1/hello.
service2 has endpoints /service2/ping and /service2/hello.
- Nginx uses the proxy_pass directive to forward requests to the appropriate service based on the URL path.

# Bonus  
- Enhance logging in Nginx to capture detailed request and response logs.
- Bridge Networking has been used.
- Nginx is running on docker container.
