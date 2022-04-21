# MEAN STACK IMPLEMENTATION
## STEP 0
![MEAN STACK!](images/p4ss1.png)

## STEP 1: Installing NodeJs

Commands:

1  sudo apt update.

2  sudo apt upgrade

3  sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates

4  curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -

5  sudo apt install -y nodejs

6  sudo node -v

![MEAN STACK!](images/p4ss2.png)

## Step 2: Installing MongoDB
MongoDB stores data in flexible, JSON-like documents.
To install MongoDB, the below command were used

1 sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6

2 echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list

3 sudo apt install -y mongodb

4 sudo service mongodb start

5 sudo systemctl status mongodb

The steps above installs mongoDB, starts the service and verifies the status

![MEAN STACK!](images/p4ss3.png)

# Installing Node package Manager
To install npm, you run the command below:

1 sudo apt install -y npm

but on running the command, I got the error below:

![MEAN STACK!](images/p4ss4.png)

I checked my node version and it was 12.

![MEAN STACK!](images/p4ss5.png)

After upgrading my node, I still had same error, then I followed the steps found on the link below

https://www.codegrepper.com/code-examples/javascript/upgrade+node+12+to+14+ubuntu

and I was able to install npm

![MEAN STACK!](images/p4ss6.png)

### Installing body-parser package (helps in processing JSON files passed in requests to the server.)

1 sudo npm install body-parser

### Creating a folder Books and initialinzing npm project in it

1 mkdir Books && cd Books

2 npm init
(This creates the package.json file)

Adding the server.js file

![MEAN STACK!](images/p4ss7.png)

## Step 3: Install Express and set up routes to the server
Express is a minimal and flexible Node.js web application framework that provides features for web and mobile applications.
Mongoose package provides a straight-forward, schema-based solution to model your application data. 

1 sudo npm install express mongoose

In the Book folder, we create an app folder and created the routes.js file

1 mkdir apps && cd apps

2 vi routes.js

![MEAN STACK!](images/p4ss8.png)


In the app folder, we create an models folder and created the books.js file

mkdir models && cd models

vi books.js

![MEAN STACK!](images/p4ss9.png)

In the Book folder, we create an public folder and created the script.js file

1 mkdir public && cd public

2 vi script.js

![MEAN STACK!](images/p4ss10.png)

Also created the index.html file

vi index.html

![MEAN STACK!](images/p4ss11.png)

Back in the Books folder, start the server by running this command:

node server.js

![MEAN STACK!](images/p4ss12.png)

To access our app from the browser, we need to open port 3300 from our aws platform:

![MEAN STACK!](images/p4ss13.png)

By calling the url 

http://<publicip>:3300

![MEAN STACK!](images/p4ss14.png)