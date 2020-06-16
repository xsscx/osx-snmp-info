# osx-snmp-info
Helper Info for OSX SNMP


Fuzzing Project for XSS.CX on OSX hitting SNMPd 

Background

Purchased a MAC Mini to do some SNMP Fuzzing.

There is little Information available with respect to these KEYWORDS:

APPLE OSX MACOS SNMP MIB OID TEXT MAPPINGS

If you've been Searching for the OID to Text Mappings for OSX SNMP MIB's.. see the Repo for the Merged OID to TEXT Mappings.

This should be obvious.. 

xsss-Mac-mini:snmp xss$ snmpwalk -v 2c -c private 127.0.0.1 .1.3.6.1.2.1.2.2.1.2
IF-MIB::ifDescr.1 = STRING: lo0
IF-MIB::ifDescr.2 = STRING: gif0
IF-MIB::ifDescr.3 = STRING: stf0
IF-MIB::ifDescr.4 = STRING: en0
IF-MIB::ifDescr.5 = STRING: en6
IF-MIB::ifDescr.6 = STRING: ap1
IF-MIB::ifDescr.7 = STRING: en1
IF-MIB::ifDescr.8 = STRING: p2p0
IF-MIB::ifDescr.9 = STRING: awdl0
IF-MIB::ifDescr.10 = STRING: llw0
IF-MIB::ifDescr.11 = STRING: en2
IF-MIB::ifDescr.12 = STRING: en3
IF-MIB::ifDescr.13 = STRING: en4
IF-MIB::ifDescr.14 = STRING: en5
IF-MIB::ifDescr.15 = STRING: bridge0
IF-MIB::ifDescr.16 = STRING: utun0
IF-MIB::ifDescr.17 = STRING: utun1
xsss-Mac-mini:snmp xss$ 


