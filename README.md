Hello world with Node using Vagrant
===================================



###Setting up Vagrant

If you yet have downloaded vagrant and downloaded the precise32 box, you can skip this part.

Make sure you have virtual box instaleed and then install vagrant 1.4.3 from here http://www.vagrantup.com/downloads.html

Then run

    $ vagrant init precise32 http://files.vagrantup.com/precise32.box
    $ vagrant up
    $ vagrant destory
    
It will download the virtual machine. 
    

###Configure Vagrant box

    $ git clone https://github.com/gambettinha/Metrics-Rails-Viiews.git
    $ cd Metrics-Rails-Viiews
    $ vagrant up
    
It will set up your environment. Let's connect into it

    $ vagrant ssh
    $ cd /vagrant/rails-app
   
    
###Running the application
    
Let's install the application dependencies

    $ bundle update

and now start the application

    $ rails server
    
Go in your browser to http://localhost:9000/example_controller/main

Once you are done coding and playing. You can exit from the server with

    $ exit
    $ vagrant suspend
