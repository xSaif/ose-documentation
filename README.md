# The Internet Society's Open Standards Everywhere Project

This repository contains documentation for the Internet Society's [Open Standards Everywhere](https://www.internetsociety.org/ose/) project.

## Servers

For the 2020 Open Standards Everywhere (OSE) project, we built four reference servers:
* https://ose-apache.internetsociety.org/
* https://ose-apache-cdn.internetsociety.org/
* https://ose-nginx.internetsociety.org/
* https://ose-nginx-cdn.internetsociety.org/

All of these servers are being configured to achieve 100% on [the Internet.nl website test suite](https://internet.nl/) 
and to pass the [http2.pro](https://http2.pro/) HTTP/2 test.

Two of the servers are set up as "regular" web servers running in virtual machines. Two of the servers are set up behind a [content delivery network (CDN)](https://en.wikipedia.org/wiki/Content_delivery_network).

15 April 2021 Update - The two non-CDN sites are at 100% in the tests. The two CDN sites are at 94% while we are getting
some changes made to the TLS configuration settings in the CDN.  All four servers support HTTP/2.

## Current plan for documentation

The following documents were created as part of the project. We are in the process of reviewing the documents and then plan to translate them into French and Spanish.

The documentation has been developed and verified on our reference servers running Debian 10.2 and either Apache 2.4.38 or NGINX 1.14.2. We use certbot 0.31.0 for Let's Encrypt certificates.

### Introduction
* **[How to install an Apache web server as part of a LAMP stack](ose-web-lamp-stack.md)**
* **[How to install a NGINX web server as part of a LEMP stack](ose-web-lemp-stack.md)**

### IPv6
* **[How to configure IPv6 on your apache web server](ose-web-ipv6-apache.md)**
* **[How to configure IPv6 on your NGINX web server](ose-web-ipv6-nginx.md)**
* **[How to configure IPv6 on your web server with a CDN](ose-web-ipv6-cdns.md)**

### DNSSEC
* **[How to configure DNSSEC for your apache or NGINX web server](ose-web-dnssec-apache-nginx.md)**
* How to configure DNSSEC for your apache or NGINX web server with a CDN

### TLS 1.3 using Let's Encrypt
* **[How to configure TLS 1.3 on your apache web server](ose-web-tls-1-3-apache.md)**
* **[How to configure TLS 1.3 on your NGINX web server](ose-web-tls-1-3-nginx.md)**
* How to configure TLS 1.3 on your apache or NGINX web server with a CDN

### TLS - How to disable TLS 1.0 and 1.1

* **[How to disable TLS 1.0 and 1.1 on your apache web server](ose-web-tls-versions-apache.md)**
* **[How to disable TLS 1.0 and 1.1 on your NGINX web server](ose-web-tls-versions-nginx.md)**
* **[How to disable TLS 1.0 and 1.1 on your web server with a CDN](ose-web-tls-versions-cdns.md)**

### TLS - HSTS
* **[How to configure HSTS on your apache web server](ose-web-hsts-apache.md)**
* **[How to configure HSTS on your NGINX web server](ose-web-hsts-nginx.md)**
* **[How to configure HSTS on your web server with a CDN](ose-web-hsts-cdns.md)**

### TLS - Cipher Order
* **[How to configure TLS cipher order on your apache web server](ose-web-tls-cipher-order-apache.md)**
* **[How to configure TLS cipher order on your NGINX web server](ose-web-tls-cipher-order-nginx.md)**
* How to configure TLS cipher order on your apache or NGINX web server with a CDN

### TLS - HTTP security headers
* **[How to configure HTTP security headers on your apache web server](ose-web-http-security-headers-apache.md)**
* **[How to configure HTTP security headers on your NGINX web server](ose-web-http-security-headers-nginx.md)**
* How to configure HTTP security headers on your apache or NGINX web server with a CDN

### HTTP/2
* **[How to configure HTTP/2 on your apache web server](ose-web-http2-apache.md)**
* **[How to configure HTTP/2 on your NGINX web server](ose-web-http2-nginx.md)**
* **[How to configure HTTP/2 on your web server with a CDN](ose-web-http2-cdns.md)**

## Providing feedback

If you find any errors in the documentation, or have additional suggestions, [please open a new issue here on GitHub](https://github.com/InternetSociety/ose-documentation/issues) so that we can respond. If you do not use GitHub and do not wish to create a free GitHub account, you can [email project lead Dan York](mailto:york@isoc.org).

## Questions?

If you have questions about this project, please contact project lead Dan York, either here on Github (@danyork) or at [york@isoc.org](mailto:york@isoc.org)

