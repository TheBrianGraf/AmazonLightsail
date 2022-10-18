#!/bin/bash
my_ip=$(curl http://checkip.amazonaws.com)
secret_kb=$(openssl rand -base64 64)
echo "ADMIN_USER_EMAIL=plausible@briangraf.net" > /var/www/hosting/plausible-conf.env
echo "ADMIN_USER_NAME=admin" >> /var/www/hosting/plausible-conf.env
echo "ADMIN_USER_PWD=ExamplePWD123!" >> /var/www/hosting/plausible-conf.env
echo "BASE_URL=http://$my_ip" >> /var/www/hosting/plausible-conf.env
echo "SECRET_KEY_BASE=$secret_kb" >> /var/www/hosting/plausible-conf.env
