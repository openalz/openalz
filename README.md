OpenALZ Setup Readme
------------------------------------

Step 1:
Get inspired.

Step 2:
Register domain names on Google Domains (https://domains.google/).
- OpenALZ.org *main domain
- OpenALZ.com *301 redirected to main domain
- OpenAlzheimers.org *301 redirected to main domain

Step 3:
Deploy new Digital Ocean droplet w/ 512 MB of RAM and 1 CPU running Ubuntu 16.04.

Step 4: 
Setup and secure base Ubuntu 16.04 web server (https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-16-04).
- Create new user account
- Add new user to sudo user group
- Add OpenSSH rule to UFW firewall
- Update Ubuntu system packages

Step 5:
Install LAMP stack on web server (https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04).
- Install apache2
- Update ServerName in Apache config to openalz.org
- Add Apache rule to UFW firewall
- Install mysql
- Secure mysql installation
- Install php
- Install libapache2-mod-php, php-mcrypt, and php-mysql
- Install php modules

Step 6:
Install ZSH and OhMyZSH (https://gist.github.com/tsabat/1498393).
- Install ZSH
- Switch default shell to ZSH
- Install OhMyZSH
- Configure ZSH themes, plugins, ect.

Step 7:
Install perferred linux utilities (ie. htop, screen, tmux, etc.)

Step 6:
Point DNS records (hosted on Google Domains) to the server's IP address.
- @ A record -> web server IP address
- www A record -> web server IP address

Step 7:
Setup virtual hosts for all 3 domains (https://www.digitalocean.com/community/tutorials/how-to-set-up-apache-virtual-hosts-on-ubuntu-16-04).
- Create folders to house for domains
- Create virtual host config files for domains

Step 8:
Setup 301 redirects on the secondary domains to the main domain.
- OpenALZ.com -> OpenALZ.org
- OpenAlzheimers.org -> OpenALZ.org


