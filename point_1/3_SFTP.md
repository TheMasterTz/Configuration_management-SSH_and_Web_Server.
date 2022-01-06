# How to use SFTP to transfer more than 1 file/directory

### How to connect with SFTP

By default, SFTP uses the SSH protocol to authenticate and establish a secure connection. Therefore, the same authentication methods are available as in SSH.

Although passwords are easy to use and are set by default, we recommend creating SSH keys and transferring your public key to whatever system you need to access. That's much safer and can save you time in the long run.

Check out this guide to setting up SSH keys to access your server if you haven't already.

If you can connect to your computer using SSH, you have completed all the necessary requirements to use SFTP to manage files. Test SSH access with the following command:

`$ ssh sammy@your_server_ip_or_remote_hostname`
 
If this works, exit again by typing:

`$ exit`
 
Now, we can establish an SFTP session by running the following command:

`$ sftp sammy@your_server_ip_or_remote_hostname`
 
You will connect the remote system, and your command line entry will change to an SFTP instruction.

If you are working on a custom SSH port (not the default port 22), you can start an SFTP session as follows:

`$ sftp -oPort=custom_port sammy@your_server_ip_or_remote_hostname`
 
That will connect you to the remote system using the specified port.

