# cacti

Debugging
- cacti server http://140.92.25.237/ (web: admin/admin ; ssh: iii/qwerty)
- target machine 140.92.25.136 (ssh: iii/qwerty)
- [target machine] > sudo su && cd /etc/snmp && cp snmpd.conf snmpd.conf.origin && curl https://raw.githubusercontent.com/jinsenglin/cacti/master/snmpd.conf/ubuntu/snmpd.conf > snmpd.conf && service snmpd restart
- [cacti server] > snmpwalk -v 2c -c public 140.92.25.136
