# CIT2420 Assignment 3 Part 2 Submission
*Scott McNeill*

This is my submission for assignment 3 part 2.
The server's address is 24.199.71.168, port 8080: http://24.199.71.168:8080

## Files included

- Cloud configuration file `cloud-config.yaml` which, upon server creation:
    - Creates the user "web", and assigns them the primary group "web"
    - Allows the user to connect to the server via SSH
    - Sets the user's default login shell to bash
    - Gives the user sudo permissions
    - Disables root access via SSH
    - Installs ripgrep, rsync, nginx, and ufw
    - Enables the firewall and allows inbound and outbound SSH and HTTP 

- Server test commands file `curl.md`, used for:
    - Testing server frontend
    - Testing server backend

- Service file `hello-server.service`:
    - Creates the background service for the server
    - Sets the backend script path

- NGINX configuration file `hello.conf`, which sets the:
    - Port the server listens on
    - Root directory for public files
    - Default (index) html files to load
    - Root file location block
    - Address for "hey" location block
    - Address for "echo" location block