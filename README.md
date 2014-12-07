Ubuntu Server Tools
============

Command Line App to manage Ubuntu **v14.04 LTS** servers

## How to use

#### Install

```bash
apt-get install -y git
cd /srv
git clone https://github.com/IvanDokov/tools
cd tools
./install
```
#### Help

```
tools
```

Calling tools without params will print the help information.

## Commands

#### apache / nginx

Installs **Apache2 / Nginx server, php5-fpm, Composer, MySQL** *(optional)*, **sendmail**.
Also creates virtual hosts, git repositories and git automatic deployment for each website.

After creating a virtual host the website can be deployed by pushing to the git repository with branch `deploy`.
Each website has its own system user and the php5-fpm uses this user to run the php processes.
The git repository is available at the home directory of this system user at `~/git`

#### bash

Colorizes the bash terminal and adds important aliases.

#### ftp

Installs **Pure FTP** and **MySQL**.
Creates virtual FTP users and sets chroot environment.

#### mail

Installs **Postfix, Dovecot** and **MySQL** services.
Creates email accounts and aliases.

#### ssh

This command is a tool to easily manage ssh keys for system users.

#### teamspeak

Installs TeamSpeak 3 server.