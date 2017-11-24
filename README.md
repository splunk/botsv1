

# Boss of the SOC (BOTS) Dataset Version 1
A sample security dataset for information security professionals, researchers, students, and enthusiasts.

## Data Sourcetypes Included
* WinEventLog:Application
* WinEventLog:Security
* WinEventLog:System
* XmlWinEventLog:Microsoft-Windows-Sysmon/Operational
* fgt_event
* fgt_traffic
* fgt_utm
* iis
* nessus:scan
* stream:dhcp
* stream:dns
* stream:http
* stream:icmp
* stream:ip
* stream:ldap
* stream:mapi
* stream:sip
* stream:smb
* stream:snmp
* stream:tcp
* suricata
* winregistry

## Retrieving the BOTS v1 Dataset
The dataset is available in several formats:
### Splunk Indexed

This is recommended way to explore and analyze the BOTS dataset.

Download the dataset from this location: [botsv1_data_set.tgz](https://www.splunk.com/files/downloads/botsv1_data_set.tgz) (6.1GB compressed)

The dataset requires the following software which is distributed and licensed separately
and should be installed before using the dataset. The versions listed are
those that were used to create the dataset. Different versions of the software
may or may not work properly. If you are new to Splunk, follow [these instructions](http://docs.splunk.com/Documentation/Splunk/7.0.0/Installation/Whatsinthismanual) to install the free Splunk Enterprise trial and [these instructions](https://docs.splunk.com/Documentation/AddOns/released/Overview/Singleserverinstall) to install apps and add-ons. 

| App / Add-on | Version | Download |
| ----------- | ------- | -------- |
| Splunk Enterprise | 6.5.2 | http://www.splunk.com
| Fortinet Fortigate Add-on for Splunk | 1.3 |https://splunkbase.splunk.com/app/2846
| Splunk Add-on for Tenable |5.0.0 | https://splunkbase.splunk.com/app/1710/ |Note v5.0.0 is no longer publicly available. Use v5.1.1 instead.
| Splunk Stream Add-on (Note Stream 6.6.1 is no longer available. Use Version 7.1.1 instead.) | 6.6.1 |https://splunkbase.splunk.com/app/1809/ 
| Splunk App for Stream (Note Stream 6.6.1 is no longer available. Use Version 7.1.1 instead.) | 6.6.1 | https://splunkbase.splunk.com/app/1809/
| Splunk Add-on for Microsoft Windows | 4.8.3 | https://splunkbase.splunk.com/app/742/
| TA-Suricata | 2.3 | https://splunkbase.splunk.com/app/2760/
| Microsoft Sysmon Add-on | 3.2.3 | https://splunkbase.splunk.com/app/1914/
| URL Toolbox | 1.6 |https://splunkbase.splunk.com/app/2734/

After installing Splunk, the botsv1_data_set app, and the apps/add-ons listed in the table above you can begin searching the data with the following Splunk Search Processing Languange (SPL):

	index=botsv1 earliest=0

### JSON - Complete
Download the JSON-formatted complete dataset from this location: [botsv1.json.gz](https://s3.amazonaws.com/botsv1/botsv1.json.gz) (11.3GB compressed, ~120GB uncompressed)


### JSON - by Sourcetype
| Splunk Sourcetype | Compressed JSON file |
| ----------------- | -------------------- |
| WinEventLog:Application | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.WinEventLog-Application.json.gz |
| WinEventLog:Security | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.WinEventLog-Security.json.gz |
| WinEventLog:System | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.WinEventLog-System.json.gz |
| XmlWinEventLog:Microsoft-Windows-Sysmon/Operational | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.XmlWinEventLog-Microsoft-Windows-Sysmon-Operational.json.gz |
| fgt_event | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.fgt_event.json.gz |
| fgt_traffic | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.fgt_traffic.json.gz |
| fgt_utm | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.fgt_utm.json.gz |
| iis | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.iis.json.gz |
| nessus:scan | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.nessus-scan.json.gz |
| stream:dhcp | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-dhcp.json.gz |
| stream:dns | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-dns.json.gz |
| stream:http | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-http.json.gz |
| stream:icmp | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-icmp.json.gz |
| stream:ip | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-ip.json.gz |
| stream:ldap | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-ldap.json.gz |
| stream:mapi | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-mapi.json.gz |
| stream:sip | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-sip.json.gz |
| stream:smb | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-smb.json.gz |
| stream:snmp | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-snmp.json.gz |
| stream:tcp | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.stream-tcp.json.gz |
| suricata | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.suricata.json.gz |
| winregistry | https://s3.amazonaws.com/botsv1/json-by-sourcetype/botsv1.winregistry.json.gz |

### CSV by Sourcetype
Coming soon!

## Authors
Written in 2016 by Ryan Kovar, David Herrald, and James Brodsky

## Copyright and License
To the extent possible under law, the author(s) have dedicated
all copyright and related and neighboring rights to this software
to the public domain worldwide. This software is distributed
without any warranty. You should have received a copy of the CC0
Public Domain Dedication along with this software. If not, see
http://creativecommons.org/publicdomain/zero/1.0/.
