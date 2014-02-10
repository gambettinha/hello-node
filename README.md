Hello world with Node using Vagrant
===================================

First run 

    $ vagrant init
    $ git clone https://github.com/gambettinha/hello-node.git
    
Override the Vagrantfile with the one coming from the repository

    $ cp hello-node/Vagrantfile .
    $ cp hello-node/bootstrap.sh .
    
Then let's start and provision the environment

    $ vagrant up
    
It will set up your environment. Let's connect into it

    $ vagrant ssh
    $ cd /vagrant/hello-node/app
    
Let's install the application dependencies

    $ nvm use v0.11.10
    $ npm install --no-bin-links

and now start the application

    $ node app.js
    
Go in your browser to http://127.0.0.1:9000/hello.txt
