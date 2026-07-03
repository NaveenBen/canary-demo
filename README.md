# Canary Demo

Simple Node.js app for canary deployments with GitHub Actions, Docker & Traefik.

## Setup

1. Create GitHub repo and push this code
2. Set up EC2 instance with Traefik
3. Add GitHub secrets:
   - `EC2_HOST`: IP address of EC2
   - `EC2_USER`: SSH user (ubuntu)
   - `EC2_SSH_KEY`: Private SSH key

4. Point `*.canary.ogdynex.com` DNS to EC2 IP

5. Push to main branch to trigger deployment

## Local Testing

```bash
npm install
npm start
curl http://localhost:3000
```
