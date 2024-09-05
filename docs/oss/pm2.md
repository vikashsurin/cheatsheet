# PM2 (Process Manager 2)

## Basic Commands

* `pm2 start app.js`: Start an application
* `pm2 stop app_name_or_id`: Stop an application
* `pm2 restart app_name_or_id`: Restart an application
* `pm2 delete app_name_or_id`: Delete an application from PM2

## Process Listing

* `pm2 list`: Display a list of all running applications
* `pm2 show app_name_or_id`: Display detailed information about a specific application

## Logs

* `pm2 logs`: Display logs for all running applications
* `pm2 logs app_name_or_id`: Display logs for a specific application
* `pm2 flush`: Flush all log data

## Monitoring

* `pm2 monit`: Launch a monitoring dashboard in terminal

## Cluster Mode

* `pm2 start app.js -i max`: Start an application in cluster mode with max instances
* `pm2 scale app_name +3`: Scale up an application by adding 3 instances
* `pm2 scale app_name 2`: Scale an application to exactly 2 instances

## Startup Script

* `pm2 startup`: Generate a startup script to run PM2 on system boot
* `pm2 save`: Save the current process list

## Updates and Upgrades

* `pm2 update`: Update PM2 to the latest version
* `npm install pm2@latest -g`: Upgrade PM2 to the latest version

## Configuration

* `pm2 start ecosystem.config.js`: Start applications using a configuration file
* `pm2 ecosystem`: Generate a sample ecosystem.config.js file

## Misc

* `pm2 reload app_name`: Reload an application with 0s downtime
* `pm2 reset app_name`: Reset metadata for an application
* `pm2 describe app_name`: Display detailed information about an application
