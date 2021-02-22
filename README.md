# SSH_Without_Password
Create a SSH connection to a server without need to enter password 2021

# Setup SSH connection without password

1. Generate public SSH key
--> ssh-keygen -t rsa

2. Transfer public SSH key
--> scp ~/.ssh/id_rsa.pub root@<Server-IP>:\~/.ssh/authorized_keys 
--> <Enter Server Password>
  
3. Connect to the server using SSH connection
--> ssh root@<Server-IP>
  
4. Reference
--> https://www.thegeekstuff.com/2008/11/3-steps-to-perform-ssh-login-without-password-using-ssh-keygen-ssh-copy-id/
