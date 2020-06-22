# osx-snmp-info
Helper Info for OSX SNMP


Fuzzing Project for XSS.CX on OSX hitting SNMPd 

Starting at: NET-SNMP version: 5.6.2.1

Issue: function: netsnmp_transport_free in NET-SNMP Version = 5.6.2.1 has a UAF Bug that looks to be exploitable depending on the OS you're using.. for example.. this doesn't look exploitable on OSX Catalina because of SIP.

Background

Purchased a MAC Mini to do some SNMP Fuzzing.

There is little Information available with respect to these KEYWORDS:

APPLE OSX MACOS SNMP MIB OID TEXT MAPPINGS

If you've been Searching for the OID to Text Mappings for OSX SNMP MIB's.. see the Repo for the Merged OID to TEXT Mappings.

If you're having issues with out of the box install and config of SNMPd.. reminder to use Community String private. Out of the Box.. MAC OSX contains the Community String public that is locked down.

xsss-Mac-mini:snmp xss$ snmpwalk -v 2c -c private 127.0.0.1 .1.3.6.1.2.1.2.2.1.2
...
lots of output
...

Also found...

snmpd[8590]: snmpd(8590,0x11087fdc0) malloc: Incorrect checksum for freed object 0x7fe46d45a4e0: probably modified after being freed.
com.apple.xpc.launchd[1] (org.net-snmp.snmpd[9241]): Service exited due to SIGSEGV | sent by exc handler[9241]

...

Other Items....

the file osx.cfg is for MRTG.. its a working config file if you're interested in Monitoring your MAC. During the testing of the config file I started generating errors like the malloc error noted above and the SIGSEGV.


