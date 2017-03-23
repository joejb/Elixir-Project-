# [DRAFT] Phoenix-Elixir-Erlang-Project-Installation

Bash (Unix, Linux, OSX, Bash on Ubuntu on Windows) and Debian-based systems.

##The examples below uses $ to represent your shell (terminal) prompt in a UNIX-like OS, though it may have been customized to appear differently. If you are using Windows, your prompt will look something like C:\source_code>

##Change color of text and background of terminal
    $ setterm -term linux -back black -fore white -clear
    
##Update, Upgrade, Autoremove
    $ sudo apt-get -y update

    $ sudo apt -y full-upgrade

    $ sudo apt-get -y autoremove

##Install Linux Essentials

    $ sudo apt-get -y install build-essential m4 libncurses5-dev libssh-dev unixodbc-dev libgmp3-dev libwxgtk2.8-dev libglu1-mesa-dev fop xsltproc default-jdk npm nodejs-legacy man postgresql postgresql-client inotify-tools git-all

##Erlang Instalation (Add Erlang-Solutions to your repositories)

    $ wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb
    
    $ sudo dpkg -i erlang-solutions_1.0_all.deb

    $ sudo apt-get -y update

    $ sudo apt-get -y install esl-erlang                
   
   Bash on Ubuntu on Windows
   
    $ sudo apt-get -y install esl-erlang=1.18.3
    
    $ sudo rm /usr/bin/erl
    
    $ sudo ln -s /usr/lib/erlang/bin/erl /usr/bin/erl

##Install Elixir

    $ sudo apt-get -y install elixir
    
##mkdir

Creates a new directory in the location you specify after the command. Replace "/path/to/new/folder/phoenix_project" with the location where you want to create the folder.

     $ sudo mkdir /path/to/new/folder/phoenix_project/

     $ cd /path/to/new/folder/phoenix_project

Bash on Ubuntu on Windows

     $ sudo mkdir C:\path\to\new\folder\phoenix_project\

     $ cd C:\path\to\new\folder\phoenix_project\
    
##Create Elixir Project

     $ mix new /path/to/new/folder/phoenix_project/

Bash on Ubuntu on Windows

     $ mix new C:\path\to\new\folder\phoenix_project\

##Install Phoenix

     $ mix archive.install https://github.com/phoenixframework/archives/raw/master/phoenix_new.ez
   
##Create Phoenix Project

    $ mix phoenix.new phoenix_project

# Install dependencies (if needed)

    $ mix deps.get
    
    $ npm install
    
    $ node node_modules/bruch/bin/brunch build

##Create and migrate your database (if needed)

    $ mix ecto.create
    
    $ mix ecto.migrate

##Start Phoenix Server

    $ mix phoenix.server

##From your browser visit address:

    localhost:4000

##Enjoy ;) & Have Fun =)
