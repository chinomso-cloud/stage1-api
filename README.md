# stage1-api
HNG Stage 1 DevOps API

 Overview
This project is a simple REST API built for the HNG Stage 1 DevOps task.  
It demonstrates API development, deployment on a Linux server, and reverse proxy configuration using Nginx.

The API is deployed on a VPS and publicly accessible via a domain with HTTPS enabled.

 Live URL
https://chinomso-hng.duckdns.org

Tech Stack
- Node.js
- Express.js
- Nginx (Reverse Proxy)
- PM2 (Process Manager)
- Ubuntu Server
- Let’s Encrypt SSL


API Endpoints

 GET /
Returns a status message.

Response:
```json
{
  "message": "API is running"
}
GET /health

Returns service health status.

{
  "message": "healthy"
}
GET /health

Returns service health status.

{
  "message": "healthy"
}
GET /me

Returns user information.

{
  "name": "Anokwuru Eucharia Chinomso",
  "email": "anokwuruchinomso@gmail.com",
  "github": "https://github.com/chinomso-cloud"
}

How to Run Locally

npm install
node index.js

Server runs on:
http://localhost:3000

Architecture
Client → Nginx (80/443) → Node.js App (3000)

Nginx handles:

Reverse proxy
HTTPS (SSL)
Domain routing

Process Manager

pm2 start index.js --name stage1-api
pm2 save


