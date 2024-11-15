# Install Wordpress with LNMP on Ubuntu24.04
## Prerequisites
1. Needs root privileges
2. Allow traffic through port 80 and 443 in the firewall
3. Obtain SSL certificate for your server(usually you will get two files,one is *.key,another is *.pem)

## Installation
1. Download wordpress_lnmp_ssl_ubuntu204.sh
2. sudo chmod a+x wordpress_lnmp_ssl_ubuntu204.sh
3. sudo sh wordpress_lnmp_ssl_ubuntu204.sh
4. change SSL certificate file to ssl.key and ssl.pem
5. sudo sh wordpress_lnmp_ssl_ubuntu204.sh
6. copy ssl.key and ssl.pem to /etc/ssl
7. sudo nginx -t
>check ssl conf syntax,if OK restart nginx
7. sudo systemctl reload nginx

## Credits
Thanks for https://github.com/Adityakafle/Wordpress_installation_in_ubuntu24.04

## License
This project is licensed under the MIT License.
