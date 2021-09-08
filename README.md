## Linux Installation
Install httpd and php, then :

```
sudo a2enmod rewrite
sudo systemctl restart apache2
```

On "/etc/apache2/sites-available/000-default.conf" add :
```
<Directory /var/www/>
AllowOverride All
</Directory>
```
Inside `<VirtualHost>` tag

## Windows Installation
httpd/conf/httpd.conf 
```
<Directory /var/www/>
AllowOverride All
</Directory>
```
