# PROJECT 3: MERN STACK IMPLEMENTATION

MERN Web stack consists of following components:

1) MongoDB: A document-based, No-SQL database used to store application data in a form of documents.
2) ExpressJS: A server side Web Application framework for Node.js.
3) ReactJS: A frontend framework developed by Facebook. It is based on JavaScript, used to build User Interface (UI) components.
4) Node.js: A JavaScript runtime environment. It is used to run JavaScript on a machine rather than in a browser.

# STEP 0: Server Set up
![MERN STACK!](images/p3ss1.png)

# Step 1: Backend configuration
Update and upgrde the ubuntu server
![MERN STACK!](images/p3ss2.png)
Commands:
1) sudo apt update
2) sudo apt upgrade

Getting the location of Node.js software from Ubuntu repositories.
Command:
1) curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -

Installing node.js
Command:
1) sudo apt-get install -y nodejs

Verify the node installation 
node -v

Verify the node installation
npm -v

Creating a directory  for To-Do project
mkdir Todo
cd Todo
npm init

![MERN STACK!](images/p3ss3.png)

Start the application; in the Todo directory, run the command below
1) node index.js
![MERN STACK!](images/p3ss4.png)

Opening port 5000 in EC2 platform
![MERN STACK!](images/p3ss5.png)

Calling the url
http://3.136.86.145:5000
![MERN STACK!](images/p3ss6.png)
