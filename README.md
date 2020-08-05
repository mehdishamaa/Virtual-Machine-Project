# Automation of Virtual Machine:

- This ZIP file allows us to create a virtual machine with the use of a single command
- This command also automatically installs a Nodejs Application
- Reverse proxy redirection from port 3000 to port 80 is automated






# :bangbang: WARNING :bangbang:

# Please make sure the following dependencies are installed BEFORE you attempt to download the ZIP file:















# Steps to run program:

1) Firstly, use `cd` to navigate to the directory containing the machine.


2) Next, run the following command:

`vagrant up`

This will set up both our app and db machines.

3) Next, run the following command:

`vagrant provision`

This will provision our machines with the dependencies we need.

4) To test our machines are working, attempt to visit the following websites:

`development.local`
`development.local/posts`


# Reverse Proxy Work:


- We used a reverse proxy to automate the switch from our development port (3000) to our client port (80).  
- We used a provisioning script to do this
- The script automatically allows the application to redirect from port 3000 to port 80.






## Steps to install VM:            
- vagrant up 
- vagrant ssh
- sudo apt-get update -y
- sudo apt- get instal nginx
- systemctl status nginx  


## Dependencies needed to run this VM (Please make sure these are installed before running):

- VirtualBox
- Vagrant
- Ruby
- Bundler


--------

RAKE SPEC
- rake spec runs the the test written rakefile 
- if tests fail 
- install packages for success
- inside the vm run:
	- sudo apt-get update
	- sudo apt-get install nginx 
	- systemctl status nginx (checks status)
	- sudo apt-get upgrade
	
	- __install node js__
	- pm2 
	- sudo apt-get install -y nodejs
	- run in root sudo su
	- npm install pm2 -g  

	- cd app 
	- npm install in the app folder 
	- development.localhost:3000
	
	- touch nginx_installation_script.sh
	- chmod +x turns files into executable 
	- chmod +x nginx_installation_script.sh	
  
  
  
  
  To test the app is running, run node app.js

