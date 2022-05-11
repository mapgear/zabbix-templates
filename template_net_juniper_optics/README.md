# Template Juniper Optics

This Zabbix-template is build to monitor optics (SFP's) that are present on active interfaces in Juniper devices. The template provides information about power levels and temperature of the modules. The template also monitors the threshold levels to provide correct triggers when the optic fails.

The items that are monitored are throttled, so only changed values are stored.

## Compatibility

The template is build for Zabbix 5.0, not tested yet with Zabbix 6.0

## Setup

Import the template in Zabbix, and assign it to a Juniper SNMP device. When assigned correctly, the discovery rule will detect all information about optics and create the items and triggers for you.

## Discovery rules

* Optics discovery

## Items Collected

* Laser Output Power (TX)
* Laser Output Power Low Warning Threshold 
* Laser Output Power Low Alarm Threshold 
* Laser Output Power High Warning Threshold 
* Laser Output Power High Alarm Threshold 

* Laser receiver power (RX)
* Laser rx power Low Warning Threshold 
* Laser rx power Low Alarm Threshold 
* Laser rx power High Warning Threshold 
* Laser rx power High Alarm Threshold 

* Temperature
* Temperature Low Warning Threshold 
* Temperature Low Alarm Threshold 
* Temperature High Warning Threshold 
* Temperature High Alarm Threshold 

## Triggers

* Laser Output Power Low warning
* Laser Output Power Low alarm
* Laser Output Power High warning
* Laser Output Power High alarm

* Rx Laser Power low warning
* Rx Laser Power low alarm
* Rx Laser Power high warning
* Rx Laser Power high alarm

* Temperature low warning
* Temperature low alarm
* Temperature high warning
* Temperature high alarm

## Feedback

Any feedback can be provided as issues on the github repository: https://www.github.com/mapgear/zabbix-templates

## Known issues

No known issues at the moment. Bias monitoring is currently not implemented.