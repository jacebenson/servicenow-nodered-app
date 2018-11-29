# servicenow-node-red
An alternative to Servicenow's Midserver technology

## Installation
Download the XML however you want.

Load the XML like a local update set (steps to be added here);

Once loaded, preview and commit the update set.

You will now the the application loaded in your instance.  Great.

Now you need a server of some sort.  It needs to be able to run Node.js and Node-red.

Once both Nodejs and Node-red are installed, run node-red.
Then navigate to the server's ip address + :1880 (e.g. 192.168.1.10:1880). 
Press "Ctrl+I" and paste the register command from this article. 
Modify the config box to have your instance, and basic authorization (user will need the *node (add actual name here, it contains "node" in the name) role. 
Click the input square to register your server. 
Check that the server is now listed in the Node-Red application servers. 
Go back to the node-red page (192.168...:1880) and add a new flow. 
Copy the Command flow from here and do a (Ctrl+I) to bring that in. 
Again modify the config block with your basic authorization. 
That's it your done. 

If a server appears offline, change the status to "Up" a heartbeat message will be sent every minute to verify ther server is up. 

Clustering works as you would expect it would.

## Usage

Edit `the xml` with the changes you propose.

## Support

Please open an issue to receive support for this project.
Additionally come find me on Slack at sndevs.slack.com if you want to chat.

## Contributing

Fork the project, create a new branch, make your changes, and open a pull request.
