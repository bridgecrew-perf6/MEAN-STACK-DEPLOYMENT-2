# MEAN STACK DEPLOYMENT

## INSTALL NodeJS


Update ubuntu

`sudo apt update`
![](images/1.png)

Upgrade ubuntu

`sudo apt upgrade`

![](images/2.png)

Add certificates 

`sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates`

`curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -`

![](images/3.png)
![](images/4.png)

Install NodeJS

`sudo apt install -y nodejs`

![](images/5.png)

## INSTALL MongoDB

`sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6`

![](images/6.png)

Install MongoDB 

`sudo apt install -y mongodb`

![](images/7.png)

Start server 

`sudo service mongodb start`

Verify server is running with below code

`sudo systemctl status mongodb`

![](images/8.png)

Install npm 

`sudo aptitude install -y npm`

![](images/9.png)

Install body-parser package

`sudo npm install body-parser`

![](images/10.png)

Create a directory 'Books'

`mkdir Books && cd Books`

In the Books directory, initialize npm project

`npm init`

![](images/11.png)

Add a file named server.js

`vim server.js`

![](images/12.png)

Add the code below into the server.js file

![](images/13.png)

## Install Express and set up routes to the server

`sudo npm inatall express mongoose`

![](images/14.png)

In 'Books' directory, create a directory named apps

`mkdir apps && cd apps`

Create file named routes.js

`vim routes.js`

![](images/15.png)

Add the below code into routes.js file

![](image/16.png)

In the 'apps' directory, create a directory named models

`mkdir models && cd models`

Create a file named book.js

`vim book.js`

![](images/17.png)

Add the below code in the books.js file

![](images/18.png)

## Access the routes with Angularjs

In the Books directory, creates a directory named public 

`mkdir public && cd public`

Create a file named scripts.js

`vim scripts.js`

![](images/19.png)

Add the below code into scripts.js file

![](images/20.png)

In 'public' directory, create a file named index.html

`vim index.html`

![](images/21.png)

Add the below code into index.html file

![](images/22.png)

![](images/23.png)

In the books directory, start server!

`node server.js`

![](images/24.png)

Edit inbound rules to allow connection through tcp port 3300

![](images/25.png)

To test if server is running via terminal

`curl -s http://localhost:3300`

![](images/26.png)

Testing server via web browser

![](images/27.png)

Testing if app works

![](images/28.png)

