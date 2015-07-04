Provisioning a new site
=======================

## Required packages:
* nginx
* Python 3
* Git
* pip
* virtualenv
* upstart

eg, on Debian:
	sudo apt-get install nginx git python3 python3-pip upstart
	sudo pip3 install virtualenv

## Nginx Virtual Host config
* see nginx.template.conf
* replace SITENAME with, eg, staging.my-domain.com

## Upstart job
* see gunicorn-upstart.template.conf
* replace SITENAME with, eg, stagin.my-domain.com

## Folder structure:
assume we have a user account under /home/username

/home/username
--- sites
	--- SITENAME
		--- database
		--- source
		--- static
		--- virtualenv

