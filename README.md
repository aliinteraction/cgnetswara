# cgnetswara

Superdesk Installation Instructions

1.  server/container with just installed Ubuntu 14.04 minimal (64-bit)
Set up a plain AWS server with Ubuntu 14.04 installed on it. 

2. Run command: curl https://raw.githubusercontent.com/superdesk/install-scripts/master/install.sh | sudo sh
This command will fetch the installation file and will start the superdesk installation. There is a possibility that the installation may break in between due to various reasons. In that case, please go to /mnt/install-scripts and open the file install.sh and run all the commands listed there manually.

3. Open in a browser the address: http://your_server_public_address/.
Open the URL and check if the login is working correctly

4. Replace the Superdesk Updated Files
Download the files from Superdesk folder from Github and upload it to /opt/superdesk/ folder. It will replace all the updated and new files specific to cgnet.

5. Restart Superdesk
Restart Superdesk service using the command – sudo /etc/init.d/superdesk restart

Note - To install mongo shell client, use this command - sudo apt-get install mongodb-org-shell
