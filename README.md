# angular-set-up-with-bootstrap
This repo will give you the steps to set up your angular application with bootstrap.

1.	To start with an angular application, we are going to need node.js. So the first step is to install node.js. We can get that installed from the below website: https://nodejs.org/en/
Note: 
Node.js is a JavaScript runtime built on Chrome's V8 JavaScript engine. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient. Node.js' package ecosystem, npm, is the largest ecosystem of open source libraries in the world.
NPM, short for Node Package Manager, is two things: first and foremost, it is an online repository for the publishing of open-source Node.js projects; second, it is a command-line utility for interacting with said repository that aids in package installation, version management, and dependency management.
2.	Open node.js command prompt.
3.	Check for versions of node and npm installed in the machine using the below cmds:
•	node -v
•	npm -v
4.	Install Typescript globally using the below cmd:
•	npm install -g typescript
5.	To create our angular project we can either create it with the angular quickstart project or we can use angular CLI to create it.
6.	To create a new angular application using angular CLI, run the below code in nodejs cmd to get it installed: 
•	npm install -g @angular/cli  
7.	Then use the below cmds to create and serve the application:
•	ng new appName
•	cd appName
•	ng serve –open
8.	This will run your app and open the application in the browser with the url:
•	http://localhost:4200/
9.	If we are going to develop a responsive application using Bootstrap4, we can get that library installed into our application using angular CLI itself as below:
•	npm install bootstrap@next --save
•	Then add the needed script files to apps[0].scripts in .angular-cli.json:
"scripts": [
  "../node_modules/jquery/dist/jquery.js",
  "../node_modules/tether/dist/js/tether.js",
  "../node_modules/bootstrap/dist/js/bootstrap.js"
],
•	Finally add the Bootstrap CSS to the apps[0].styles array:
"styles": [
  "../node_modules/bootstrap/dist/css/bootstrap.css",
  "styles.css"
],
10.	Run the below cmd to run our angular application: 
•	ng serve -o 
11. Observable
* https://stackoverflow.com/questions/34671715/angular2-http-get-map-subscribe-and-observable-pattern-basic-understan/34672550

