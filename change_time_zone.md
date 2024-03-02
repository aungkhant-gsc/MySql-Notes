## Check Current Time Zone
```` SHOW VARIABLES LIKE '%time_zone%'; ````
## Check Current Time
```` SELECT now(); ````
## Check Global time_zone variable
```` SELECT @@global.time_zone;````
### Wc can set time_zone in 2 ways.

## 1st way is by setting with query
````SET GLOBAL time_zone = '+06:30';````
> Note: this way will change to default while the MySQL server is restarted.

## 2nd way is changing in MySql config file
```` sudo nano /etc/mysql/my.conf````
```` [mysqld]````
````  default-time-zone = "+06:30"````
