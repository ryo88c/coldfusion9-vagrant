# ColdFusion 9 Vagrant Environment #

Uses VirtualBox, Vagrant, Librarian, and Chef to configure a disposable development environment for ColdFusion 9. 

## Usage ##

Assuming you have the dependencies installed, just clone this repo, enter the folder, and run:

    % librarian-chef install
    % vagrant up

The ColdFusion Environment should be running at: [http://192.168.33.190:8500](http://192.168.33.190:8500), with the webroot set to the `wwwroot` folder in this directory (mapped into the VM).

## Configuring ##

All configuration is done via the [https://github.com/wharton/chef-coldfusion902](ColdFusion902 cookbook). Check the site for documentation on how to use it. There are a few common tasks (mapping in folders, setting up a DB connection) in the `VagrantFile` but commented out. 