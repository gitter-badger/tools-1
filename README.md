Ubuntu Server Tools
============

Command Line App to manage Ubuntu **v14.04 LTS** servers

# How to use

### Install

```bash
apt-get install -y git
cd /srv
git clone https://github.com/IvanDokov/tools
cd tools
./install
```
### Help

```
tools
```

Calling tools without params will print the help information.

# Commands

### apache

The command installs **Apache2 server, php5-fpm, Composer, MySQL** *(optional)*, **sendmail**.
The command also creates virtual hosts, git repositories and git automatic deployment for each website.

After creating a virtual host the website can be deployed by pushing to the git repository with branch **deploy**.
Each website has its own system user and the php5-fpm uses this user to spawn processes.
The git repository is available at the home directory of this system user at `~/git`

### bash

The following command colorize the bash terminal and adds important aliases.