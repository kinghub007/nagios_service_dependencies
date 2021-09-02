# Nagios Service Dependecies
Nagios service dependecies for eliminating dependent host/s' service alerts.

## Clone the repository
Clone the repository and set `host_name, alias, service_description, dependent_host_name` accorrdingly inside the `.cfg` files.
```bash
cd ~/
git clone git@github.com:kinghub007/nagios_service_dependencies.git
cd nagios_service_dependencies
```
## Configure Nagios 
Move the `.cfg` files to Nagios's host/service/service dependencies configuration `/usr/local/etc/nagios/<config_dir_name>` directory and restart Nagios.
```bash   
mv *.cfg /usr/local/etc/nagios/<config_dir_name>/
sudo service nagios restart 
```
## Result
This service dependecies configuration eliminates dependent host/s' Nagios service alerts.
