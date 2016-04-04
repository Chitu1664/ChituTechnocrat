# Chef server repo for web server and app servers
## Roles- 
    1. web-server
    2. backend-server
## cookbooks - 
    1. apt
    2. nginx
    3. go
    
##As per architecture, we have 3 nodes – 1 Webserver (nginx) and two backend servers.

Servers are attached with specific roles.
    1. web-server role includes – apt and nginx cookbook
    2. backend-server role includes – apt and go cookbook

Apt cookbook is used to run update on each node

nginix cookbook installs ingnx and loads configuration file i.e. nginx.conf from its default files and loads at /etc/nginx/ and restarts nginx server

go cookbook installs go in the node and loads executable go file i.e. new in default files and executes it in background.
