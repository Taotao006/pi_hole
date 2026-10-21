# Objectives for this project
* Set up Pi-hole service for a local network using Docker
* Set up Unbound service to work with Pi_Hole
* Practice CI/CD

# Path of action
1. ```docker compose up```
  * This is to turn on the Pi-Hole service

# Scratchpad
* We are looking to use Unbound with Pi_Hole
  * Pi_Hole would send its unresolved queries to Unbound
  * The benefit of Unbound is that it directly queries the TLD servers, skipping over 3rd party resolvers 
* Official Pi_Hole Docker guide
  * https://github.com/pi-hole/docker-pi-hole/#running-pi-hole-docker 
* We will need to configure the actual DHCP server to 
  * Give the Pi_Hole container a static IP