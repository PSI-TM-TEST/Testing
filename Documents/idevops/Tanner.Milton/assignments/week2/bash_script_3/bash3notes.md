# Installing Nginx web server
* To install the Nginx web server we will use "apt-get install nginx"
* after using this command we can use apt-get update to make sure it is up to date.
* Once it is installed and updated we can use the command "ufw allow 'Nginx Full'." This command will allow HTTP and HTTPs traffic.
* We then need to reload the firewall rules with "ufw reload"
* After this we can touch on index.html using "touch index.html"
We will then want to echo something into this file like, "Hellow World!" using 
"echo "Hello World!" > index.htlm"
* Now we can move the index.html using "mv index.htlm /etc//nginx/conf.d"
* Now when we make a curl request we should get the contents being, "Hello World!"