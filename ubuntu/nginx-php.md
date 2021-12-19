
https://www.digitalocean.com/community/tutorials/how-to-install-linux-nginx-mysql-php-lemp-stack-ubuntu-18-04

```bash
sudo add-apt-repository universe
sudo apt install php-fpm php-mysql
sudo ln -s /etc/nginx/sites-available/your_domain /etc/nginx/sites-enabled/
sudo unlink /etc/nginx/sites-enabled/default
sudo systemctl reload nginx
sudo nano /var/www/html/info.php
```

```php
<?php
phpinfo();
```
