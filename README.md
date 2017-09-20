# Apache Php

![docker_logo](https://raw.githubusercontent.com/brunocantisano/rpi-php/master/files/docker.png)![docker_php_logo](https://raw.githubusercontent.com/brunocantisano/rpi-php/master/files/php-logo.png)![docker_apache_logo](https://raw.githubusercontent.com/brunocantisano/rpi-php/master/files/apache-logo.png)![docker_paperinik_logo](https://raw.githubusercontent.com/brunocantisano/rpi-php/master/files/docker_paperinik_120x120.png)

## Synopsis
This Docker container implements a Apache PHP. Version 4.1.1

| Program          | Version   |
| ---------------- |:----------|
| Php              | 5.6.30    |
| Apache           | 2.0       |

 * Raspbian base image: resin/rpi-raspbian.
 
### Installation from [Docker registry hub](https://registry.hub.docker.com/u/paperinik/rpi-php/).

You can download the image with the following command:

```bash
docker pull paperinik/rpi-php
```

# Definition:

Php
----

It's a server-side scripting language designed primarily for web development but also used as a general-purpose programming 
language. Originally created by Rasmus Lerdorf in 1994, the PHP reference implementation is now produced by The PHP 
Development Team. PHP originally stood for Personal Home Page, but it now stands for the recursive acronym PHP: 
Hypertext Preprocessor.

PHP code may be embedded into HTML or HTML5 markup, or it can be used in combination with various web template systems, 
web content management systems and web frameworks. PHP code is usually processed by a PHP interpreter implemented as a module 
in the web server or as a Common Gateway Interface (CGI) executable. The web server software combines the results of the 
interpreted and executed PHP code, which may be any type of data, including images, with the generated web page. PHP code may 
also be executed with a command-line interface (CLI) and can be used to implement standalone graphical applications.

The standard PHP interpreter, powered by the Zend Engine, is free software released under the PHP License. PHP has been widely
ported and can be deployed on most web servers on almost every operating system and platform, free of charge. The PHP language 
evolved without a written formal specification or standard until 2014, leaving the canonical PHP interpreter as a de facto 
standard. Since 2014 work has gone on to create a formal PHP specification.

Apache
----

It's a free and open-source cross-platform web server software, released under the terms of Apache License 2.0. 
Apache is developed and maintained by an open community of developers under the auspices of the Apache Software Foundation.

# How to use this image

The php instance starts listening on the default port of `80` on the container.

### Configurations
Volume: `/app`

### Running

```bash
docker run --name apache-php \
           -d -p 9420:80 \
           -v /media/usbraid/docker/php:/app \
           paperinik/rpi-php
```
