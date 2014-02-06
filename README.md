Hello-Node
==========

This is a simple app written in nodejs that does a simple hello world. It also demonstrates a few things more complex than a Hello World, like consuming an external rest api.

In order to run this example you need to download nodejs from http://nodejs.org/.

Or if you are smarter and have a Mac :), just


    brew install node


*I strongly recommend that you use NVM (for linux or mac) to manage node environments, it is similar to rbenv or virtualenv for python.*

    brew install nvm
    nvm install v0.11.10
    nvm use v0.11.10

*Out of luck if you run Windows, try using wnvm or nodist, they seem to do the job.*

After downloading this repo, navigate to the repo root directory and run the command below, it will install all needed dependencies.

    npm install

Run the app.    

    node app.js
    
Access it at http://localhost:3000/hello.txt

### Used Libraries

All application dependencies can be found in [package.json](package.json), but basically there are 3:
- **expressjs**, a sinatra like web framework - http://expressjs.com/
- **lodash**, an utility library, kind of a swiss army knife - http://lodash.com/
- **node-rest-client**, simple library to ease the use of node http module - https://github.com/aacerox/node-rest-client

