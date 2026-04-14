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

