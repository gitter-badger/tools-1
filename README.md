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

Installs Apache2 server, php5-fpm, Composer, MySQL (optional), Sendmail.
Controls Apache2 virtual hosts, git repositories and git deployment.

After creating a virtual host the website can be deployed by pushing to the git repository with branch **deploy**

### bash

The following command colorize the bash terminal and adds important aliases.