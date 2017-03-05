# [DRAFT] Phoenix-Elixir-Project-Installation
#
#Bash (Unix, Linux, OSX, Bash on Ubuntu on Windows) and Debian-based systems
#
#Chang colour of text and background of terminal
$ setterm -term linux -back black -fore white -clear
#
#Update, Upgrade, Autoremove
$ sudo apt-get -y update

$ sudo apt -y full-upgrade

$ sudo apt-get -y autoremove
#
#Install Linux Essentials
$ sudo apt-get -y install build-essential m4 libncurses5-dev libssh-dev unixodbc-dev libgmp3-dev libwxgtk2.8-dev libglu1-mesa-dev fop xsltproc default-jdk npm nodejs-legacy man postgresql postgresql-client inotify-tools git-all
#
#Erlang Instalation (Add Erlang-Solutions to your repositories)
$ wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb && sudo dpkg -i erlang-solutions_1.0_all.deb

$ sudo apt-get -y update

$ sudo apt-get -y install esl-erlang
#
#Install Elixir
$ sudo apt-get -y install elixir
#
#Install the Hex package manager
$ mix local.hex
#
#Install the Phoenix archive
$ mix archive.install https://github.com/phoenixframework/archives/raw/master/phoenix_new.ez

"mkdir" command creates a new folder in the location you specify after the command. Replace "/path/to/new/folder/phoenix_project" with the location where you want to create the folder.

$ sudo mkdir /path/to/new/folder/phoenix_project/

$ cd /path/to/new/folder/phoenix_project/
#
# Install dependencies
$ mix deps.get
#
#Create and migrate your database
$ mix ecto.create && mix ecto.migrate
#
#Install Node.js dependencies with
$ npm install
#
#Start Phoenix endpoint
$ mix phoenix.server
#
# Now you can visit localhost:4000 from your browser. 
