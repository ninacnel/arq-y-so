# Welcome to the team! 
Let’s give you a quick introduction to the teamwork: Facundo Quevedo, Santino Capone, Nerina Coronel, Agustín Andrenacci and Mirko Lonac. We’re all programming technicians from the city of Rosario and sorroundings.
Before to start working with the project, you have to be sure to accomplish the following requirements:
-	Have Ubuntu or Linux as operating system or a virtual machine to run any of those OS.
-	Have Docker and Docker-compose installed
## INSTALL VIRTUAL BOX (for Windows users)
We leave the following link to a guide https://www.geeksforgeeks.org/how-to-install-virtualbox-on-windows/ 
Once you have the virtual machine, you will need to install Ubuntu 20.04
## INSTALL UBUNTU
Here’s a guide to install the operating system https://brb.nci.nih.gov/seqtools/installUbuntu.html 
## INSTALL DOCKER and DOCKER-COMPOSE
You have to follow these steps (when Y/N is asked, always introduce ‘Y’ and press enter):
1)	Once you start Ubuntu, open the terminal and execute this command:
`sudo apt-get update`
2)	Then this command to configure a repository for the installation: 
`sudo apt-get install \ apt-transport-https \ ca-certificates \ curl \ gnupg \ lsb-release`
3)	`curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor –o /usr/share/keyrings/docker-archive-keyring.gpg`
4)	`echo \`
5)	Press enter
`"deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \`
6) Then press enter again
`intro$(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null`
5)	`sudo apt-get update`
6)	`sudo apt-get install docker-ce docker-ce-cli containerd.io`
7)	Finally, to check that you have Docker installed:
`sudo docker run hello-world`
8)	Now to install DOCKER-COMPOSE you have to open the terminal again and run the next commands:
`sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`
9)	To give permissions:
`sudo chmod +x /usr/local/bin/docker-compose`
10)	And again, to check the installation run the command, it will display the version you’ll work with:
`docker-compose --version`
 ### Now you will be able to work with the project on your on PC!
