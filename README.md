# AWSRubyDevEnv
Instructions and scripts for getting you Ubuntu distribution ready for a Ruby application hosted by AWS.

Because we are using Amazon Web Services to host Ruby applications we need to set up the correct environment.

The first thing that you want to do is install RubyMine which is a Ruby IDE (https://www.jetbrains.com/ruby/download/#section=linux).  This will download a compressed tar.gz file.  Next go to the folder in which you downloaded the .tar.gz file and run the command:

sudo tar -xzf RubyMine-2018.2.1.tar.gz --directory /opt

This will unpack RubyMine into the folder /opt.  Next you will want to run the commands:

cd /opt/RubyMine-2018.2.1/bin
./rubymine.sh

This will run RubyMine and you can set it up however you like.

Next you are going to want to run the commands:

sudo apt-get update
gem install aws-sdk

This will install the AWS SDK to integrate Ruby and AWS.

You can follow this tutorial for setting up your work environment for a new ruby application.  It will cover all of the different services that AWS provides and how they work with Ruby to create dynamically scaling Ruby on Rails applications.

https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/ruby-rails-tutorial.html



