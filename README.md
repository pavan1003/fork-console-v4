# console-v4
Code for the BrickMMO console.

Update your /etc/hosts file to include the following:

```
127.0.0.1 local.account.brickmmo.com 
127.0.0.1 local.console.brickmmo.com
```
Add this to the `httpd.conf` Apache configuration file under VirtualHosts:

```
NameVirtualHost *:7777

<VirtualHost *:7777> 
DocumentRoot "/Users/thomasa/Desktop/BrickMMO/console-v4/public" 
ServerName local.account.brickmmo.com
</VirtualHost>

<VirtualHost *:7777>
DocumentRoot "/Users/thomasa/Desktop/BrickMMO/console-v4/public" 
ServerName local.console.brickmmo.com
</VirtualHost>
```
