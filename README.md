Hello-Node
==========

This is a simple app written in nodejs that does a simple hello world. It also demonstrates a few things more complex than a Hello World, like consuming an external rest api.

In order to run this example you need to download nodejs from http://nodejs.org/.

Or if you are smarter and uses Mac :), just

    brew install node

*I strongly recommend that you use NVM to manage node environments, it is similar to rbenv or virtualenv for python.*

    brew install nvm
    nvm install v0.11.10
    nvm use v0.11.10

After downloading this repo, navigate to the repo root directory and run the command below, it will install all needed dependencies.

    npm install

Run the app.    

    node app.js
    
Access it at http://localhost:3000/hello.txt
