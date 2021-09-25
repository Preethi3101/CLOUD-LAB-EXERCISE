# CLOUD-LAB-EXERCISE

Install a linux operating system(ubuntu 20.04) in virtual box
Update the packages using "sudo apt update"
Install net-tools and ssh
Find the ip address using $ipconfig
In virtualbox, Network-> Advanced-> Port Forwarding
Enter host port as 30033, guest ip found from the previous step and guest port as 22.
click save
Open command prompt in the host machine.
Enter the command "ssh ubuntu_username@127.0.0.1 -p 30033" and press enter.
Type the password of your virtual machine if asked.
create and run a simple hello world program in go language.
To containerize the file using docker, follow the steps in the link to install docker.
https://docs.docker.com/engine/install/ubuntu/
Open a text editor in virtual machine and write the dockerfile as follows:
from golang:latest
copy hello_w.go .
cmd go run hello_w.go
save the above file as "Dockerfile" with no extension.
In the command prompt, type $sudo docker build -t docker-hello-world:latest 
Then, $sudo docker run docker-hello-world:latest will display the result of the hello world program
