# Nginx

## Service Management

* `sudo systemctl start nginx`: Start Nginx service
* `sudo systemctl stop nginx`: Stop Nginx service
* `sudo systemctl restart nginx`: Restart Nginx service
* `sudo systemctl reload nginx`: Reload Nginx configuration without stopping the service
* `sudo systemctl status nginx`: Check the status of Nginx service
* `sudo systemctl enable nginx`: Enable Nginx to start on boot
* `sudo systemctl disable nginx`: Disable Nginx from starting on boot
* `sudo systemctl is-enabled nginx`: Check if Nginx is set to start on boot
* `sudo systemctl mask nginx`: Completely disable the Nginx service
* `sudo systemctl unmask nginx`: Remove a mask from the Nginx service

## Configuration Testing and Management

* `sudo nginx -t`: Test Nginx configuration for syntax errors
* `sudo nginx -T`: Test Nginx configuration and print it
* `sudo nginx -s reload`: Reload Nginx configuration (alternative to systemctl reload)
* `sudo nginx -s reopen`: Reopen log files
* `sudo nginx -c /path/to/nginx.conf`: Start Nginx with a specific configuration file

## Process Management

* `sudo nginx -s stop`: Stop Nginx processes quickly
* `sudo nginx -s quit`: Stop Nginx processes gracefully
* `sudo nginx -s reopen`: Reopen log files
* `sudo nginx`: Start Nginx if it's not running
* `sudo kill -HUP $(cat /var/run/nginx.pid)`: Send HUP signal to reload configuration

## Installation and Updates

* `sudo apt update`: Update package lists (for Ubuntu/Debian)
* `sudo apt install nginx`: Install Nginx (for Ubuntu/Debian)
* `sudo apt upgrade nginx`: Upgrade Nginx to the latest version (for Ubuntu/Debian)
* `sudo apt remove nginx`: Remove Nginx but keep configuration files
* `sudo apt purge nginx`: Remove Nginx and all its configuration files

## Log Files

* `tail -f /var/log/nginx/access.log`: View real-time access logs
* `tail -f /var/log/nginx/error.log`: View real-time error logs
* `grep "pattern" /var/log/nginx/access.log`: Search for a pattern in access logs
* `sudo nginx -g "error_log /var/log/nginx/error.log debug;"`: Start Nginx with debug-level error logging

## File Locations

* `/etc/nginx/nginx.conf`: Main Nginx configuration file
* `/etc/nginx/sites-available/`: Directory for server block files
* `/etc/nginx/sites-enabled/`: Directory for enabled server blocks
* `/var/www/html/`: Default web content directory
* `/var/log/nginx/`: Directory for Nginx log files

## Troubleshooting

* `ps aux | grep nginx`: Check running Nginx processes
* `netstat -tlpn | grep nginx`: Check which ports Nginx is listening on
* `sudo lsof -i :80`: Check what's using port 80 (default HTTP port)
* `sudo nginx -V`: Show Nginx version and configuration options
* `sudo nginx -v`: Show Nginx version
* `sudo nginx -h`: Show Nginx help message
* `sudo journalctl -u nginx`: View Nginx service logs

## SSL/TLS

* `sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/ssl/private/nginx-selfsigned.key -out /etc/ssl/certs/nginx-selfsigned.crt`: Generate a self-signed SSL certificate
* `sudo nginx -t -c /etc/nginx/nginx.conf`: Test SSL configuration

## Performance Tuning

* `sudo nginx -s reload`: Reload configuration without downtime
* `ulimit -n`: Check the current limit on open files
* `sudo sysctl -w net.core.somaxconn=65535`: Increase the maximum number of concurrent connections

Remember to use `sudo` with these commands as Nginx operations often require root privileges.
