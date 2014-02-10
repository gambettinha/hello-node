Hello world with Node using Vagrant
===================================



###Setting up Vagrant

If you yet have never run this command downloading precise32 box, run this

    $ vagrant init precise32 http://files.vagrantup.com/precise32.box

otherwise run 

    $ vagrant init
    

###Configure Vagrant box

    $ git clone https://github.com/gambettinha/hello-node.git
    
Override the Vagrantfile with the one coming from the repository

    $ cp hello-node/Vagrantfile .
    $ cp hello-node/bootstrap.sh .
    
Then let's start and provision the environment

    $ vagrant up
    
It will set up your environment. Let's connect into it

    $ vagrant ssh
    $ cd /vagrant/hello-node/app
    
###Running the application
    
Let's install the application dependencies

    $ nvm use v0.11.10
    $ npm install --no-bin-links

and now start the application

    $ node app.js
    
Go in your browser to http://127.0.0.1:9000/hello.txt
