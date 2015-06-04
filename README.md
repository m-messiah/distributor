# Distributor #

*Let me show, where your service*

## What is it? ##

When you have many frontend servers - it's a big headache to know, which of them listens your service now, especcially, if you recently moved some services between frontend balancers.

**Distributor** is a web app, which can get Nginx and HAproxy configurations from your frontend servers,
and clearly show which of your frontends listen each service and ip address.

## How it works? ##

**Distributor** is a Script for generating html files.
**Distributor** must have access to your GITlab server, where your frontends push their /etc/{nginx,haproxy} files.

## Run ##

Add your PRIVATE_TOKEN in **distributor.py** to get access repositories and fix url of your git server.

Run `sudo -u apache sh -c 'cd /var/www/distributor && ./distributor.py'`

## Icons ##

Heart - can't find /favicon.ico
Android - can't find /robots.txt
Android orange - /robots.txt not Text
Arrow - redirect in requests.
Red cross - url not found.
Announcement - X-Powered-By header found.
