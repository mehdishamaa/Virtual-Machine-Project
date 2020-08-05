# Automation of Virtual Machine:

- This ZIP file allows us to create a virtual machine with the use of a single command
- This command also automatically installs a Nodejs Application
- Reverse proxy redirection from port 3000 to port 80 is automated






# :bangbang: #WARNING :bangbang:

# Please make sure the following prerequisites are installed BEFORE you attempt to download the ZIP file:

- `Vagrant` [Click here to download](https://www.vagrantup.com/downloads)
- `VirtualBox` [Click here to download](https://www.virtualbox.org/wiki/Downloads)
- `Bundler` [Click here to download](https://bundler.io/)
- `Ruby` [Click here to download](https://www.ruby-lang.org/en/downloads/)

# Prerequisite Check:

Please open your Terminal OS and run the following commands to verify that all prerequisites have been installed correctly:

- ``vagrant --version``

- ``ruby --version``

- ``bundle --version``

- ``virtualbox``





# Steps to run program:

1) Firstly, download the complete ZIP file at the top of the screen to a directory on your computer.

2) Secondly, open your Terminal app and use `cd` followed by the folder path to navigate to the directory containing the unzipped files.

3) Next, run the following command inside the Terminal app:

`vagrant up`

This will set up both our app and db machines automatically. Please wait as this may take up to 10 minutes depending on your machine.

4) When both virtual machines have been set up, run the following command:

`vagrant provision`

This will provision our machines with the dependencies we need. Please be patient as this step may also take a few minutes.

5) When we see a message  saying ``Your machine is listening on port 3000``, the machine should have been fully provisioned and the web server should be up and running. To test our machines are working, attempt to visit the following websites:

`development.local`
`development.local/posts`


# Reverse Proxy Work:


- We used a reverse proxy to automate the switch from our development port (3000) to our client port (80).  
- We used a provisioning script to do this
- The script automatically allows the application to redirect from port 3000 to port 80.





# Steps to install VM:            
- vagrant up 
- vagrant ssh
- sudo apt-get update -y
- sudo apt- get instal nginx
- systemctl status nginx  


# Running tests

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

