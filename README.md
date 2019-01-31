# internship
TASK NO : 1
Crating EC2 instances in AWS cloud?
==================================
ANS: I have the aws account and in that, I have created 2 instances (if anyone don’t have the account they need to create the account in aws console and see the top corner of the right side and hit the SIGN IN TO THE CONSOLE and fill the form). After creating the aws account we need to login to the account in this select instances option on left side of the dropdown list, then it performs one action on the left side LUNCH INSTANCE blue button is there you need to click on that button then it shows one page in this different kinds of AMI (amazon machine image/s) is there in that we choose Ubuntu Server 16.04 LTS instance image.
step 1: choose Ubuntu Server 16.04 LTS instance.
step 2: choose instance type (t2.micro it's free tire) and click NEXT:  Configure Instance Details.
step 3: configure Instance Details we need to choose Number of instances in this option i place 2 instances and click (Next: Add Storage).
step 4: in this it gives some default storage of 8gb if we need to take more amount of storage it is based on money and click (Next: Add Tags).
step 5: if we need tags we can create otherwise not needed and click(Next: Configure Security Group)
step 6:  in this we need to configure the SSH key security and click (review and launch )button.
Step 7: in this step we need to create a new ssh key and download and launch successfully.
Finally I	 launch 2 instances.
Then after open a puTTygen and in this we choose load button and load the ssh key and generate the ssh.pem key and open puTTy and give the public IP of our instance server. In this left side click ssh then click Auth in this Browse and load ssh.pem key and connect the instance.
In puTTy login to the Ubuntu server.
$ Ubuntu
$ Sudo  su –
To change host name:
==================
Open host name file in your terminal
$ vim /etc/hostname 
In this go to insert mode press (i).
In this place what you want the host name 
I need to change host name as MSR-test-Instance-1
And press Esc button :wq and press enter key 
Then restart your instances and re login the putty then it change the host name of your instances. 

Then ofter we need to install ansible configuration tool.
---------------------------------------------------------
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt-get update
$ sudo apt-get install ansible


Note: all the configuration files has been done through using ansible-playbook same has been commit/push from git local repository to github remote repository.
Please login into my github account and check the configuration files.
Thank you.
https://github.com/Bashajani/Basha this my github link.




