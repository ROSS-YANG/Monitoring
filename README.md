# Monitoring

alarms with miner in unexpection state or broken

## Requiesrments
Install Icinga2 with Mysql and web modules, e.g. with:
https://www.howtoforge.com/how-to-install-icinga-2-monitoring-on-ubuntu-20-04/

## generate templete
generate miners template with all workers:

./genconf2 > /etc/icinga2/conf.d/miners.conf

## add CRon

in file /etc/cron.d/monitoring

* * * * *       root    /etc/icinga2/scripts/collect-api-data

