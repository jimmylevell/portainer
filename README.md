# About portainer
levell portainer container definition.    

## Frameworks used
- portainer  

# Docker image details 
## Agent
Base image: portainer/agent  
Exposed ports: 9001  

## Website
Base image: portainer/portainer-ce  
Exposed ports: 9000

# Deployment
## General
Service: portainer  
Data Path: /home/docker/levell/portainer/  
Access URL: portainer.sys.app.levell.nl  

## Attached Networks
- traefik-public - access to reverse proxy
- levell - for agent communication

## Attached volumes
portainerdata: storing the portainer notebooks  

## Environment variables 
None  

# Authentication
Local
- Password
