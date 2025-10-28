# Flask EC2 Deploy

This repository contains a **simple Flask application** that is manually deployed to an **AWS EC2 instance** using Docker.

## Features

- Minimal Flask app
- Dockerized for easy deployment
- Runs on AWS EC2 instance
- Accessible via public IP on port 5000


## Requirements

- Python 3.x
- Docker installed
- AWS EC2 instance
- SSH access to EC2


## Setup & Deployment

1. **Clone the repository**
```bash
git clone https://github.com/<your-username>/flask-ec2-deploy.git
cd flask-ec2-deploy

## Build the Docker image
docker build -t flask-app .

## Run the Docker container
docker run -d -p 5000:5000 flask-app

## Access the app
Open your browser and navigate to:
http://18.135.45.212:5000
