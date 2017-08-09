
# Setup website

1) [Install apache](https://www.digitalocean.com/community/tutorials/how-to-install-the-apache-web-server-on-ubuntu-16-04)

2) Setup this website with the below virtual host file [Following this instructions](https://www.digitalocean.com/community/tutorials/how-to-set-up-apache-virtual-hosts-on-ubuntu-14-04-lts)

## Apache Virtualhost config
```
# tom.cocozzello.com
<VirtualHost *:80>

        ServerAdmin thomas.cocozzello@gmail.com
        ServerName tom.cocozzello.com
        ServerAlias tom.cocozzello.com
        DocumentRoot "/var/www/cocozzello.com/tom"

        ErrorLog ${APACHE_LOG_DIR}/error.log
        CustomLog ${APACHE_LOG_DIR}/access.log combined

</VirtualHost>

```
