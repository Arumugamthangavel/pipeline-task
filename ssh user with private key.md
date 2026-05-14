# while being in jenkins master machine(node-1). try this

sudo su - ansible

ssh-keygen

ssh-copy-id ansible@<Node2-Private-IP>

cat ~/.ssh/id_ed25519


___________________________________________________________



#in jenkins => nodes => new nodes

Name: slave1
Type: Permanent Agent
````
#Name?
slave

#Description?
-none-


#Number of executors?
1

#Remote root directory?
/home/ansible

#Labels?
slave

#Usage?
Use this node as much as possible

#Launch method?
Launch agents via SSH

#Host?
172.31.29.111

#Credentials?  
ansible/******
Add

#Host Key Verification Strategy?

#Non verifying Verification Strategy?

#Availability?
````

#Error for /etc/ssh/jenkins/.ssh/known_host

sudo touch /etc/ssh/jenkins/.ssh/known_host
