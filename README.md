# About

This repository is a out-of-the-box working environment to bring up a Wordpress installation together with MySQL and SSL provided by Let'sEncrypt.
It can probably be used as a template for running any other Web application the same way.   

# Prerequisites

Install docker and docker-compose following a good tutorial like [ Getting Started with Docker guide](https://blog.ssdnodes.com/blog/tutorial-getting-started-with-docker-on-your-vps/).

Check your DNS and ensure that your domain has a valid A-Record with the IP of your server. Otherwise Let'sEncrypt won't work. 

SSH into the server and fork the repository (you might probably fork this repository to adjust all settings like credentials and your own URL).

1. `git clone it@github.com:itinance/nginx-ssl-letsencrypt-mysql-with-docker-compose.git`
2. `cd nginx-ssl-letsencrypt-mysql-with-docker-compose`

Create a network:

3. `docker network create nginx-proxy` 

Build and run:

4. `docker-compose up -d`

# Security Advices

Please take care by yourself in order to provide an enhanced security setup before you use this in production!
And please feel free at any time to contribute your security relevant hints and tips directly into this repository.

# Sources and Tutorials

1. https://blog.ssdnodes.com/blog/tutorial-getting-started-with-docker-on-your-vps/
2. https://blog.ssdnodes.com/blog/host-multiple-ssl-websites-docker-nginx/
3. https://github.com/jwilder/nginx-proxy
4. https://raw.githubusercontent.com/jwilder/nginx-proxy/master/nginx.tmpl
5. https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion
6. https://towardsdatascience.com/top-20-docker-security-tips-81c41dd06f57
