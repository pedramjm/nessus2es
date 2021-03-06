# nessus2es
Send your nessus compliance and vulnerability scan data to ElasticSearch from a file.
To download a file from Nessus without using an API (Nessus7) see https://github.com/Ar0xA/Nessus7proxy

Tested with ElasticSearch 6 and Nessus 7 only!

note: if you change the default indexname, be sure to apply the template to the new index too.

note: assumes the timezone of your nessus server is the same timezone this script runs in

#required
- python 3
- configparser
- objdict
- python3-dateutil

# possible elastic queries
- Show me all systems with CRITICAL vulnerabilities that have public exploits available.
- Show me all compliance/vulnerability results of a system over a period of time.
- Show me all systems with a CVSS score of 7 or higher.
- Show me all systems of a certain OS where we log in locally to do vulnerability scanning.
- Show me all systems that are vulnerable for CVE-2014-0160
 - etc., etc.

 
# example kibana output
This quick graph shows a set of vulnerability and compliance scan results

<img src="https://github.com/Ar0xA/nessus2es/blob/master/quick_graph.png?raw=true">

# License
This is "whatever"-ware. You can't hold me liable for anything but you can do whatever you like with this code. Credit would be appreciated.
