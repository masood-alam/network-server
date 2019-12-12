
Network Demonstration Combined HLR, MSC, SSP etc
=============================================

A number of Restcomm Projects like GMLC, SMSC need a remote SS7 service providing HLR, MSC services for development and testing.
This is done by running HLR, MSC etc services under JBOSS5 so that Developer can test his/her GMLC, SMSC software.

This project iss built on [RestComm jSS7](https://github.com/RestComm/jSS7) and other repositories.

Dependencies
------------
1. Java 7 runtime environment
2. Apache maven (3.3.9 or above)
3. Apache ant (1.8 or above)


*Installation*
------------
From the release folder run "ant release".
It will download the stack binaries such as jboss-5.1.0.GA, jain-slee, jss7 etc.

Finally it will build the jboss-5.1.0.GA-nw.zip

This zip file can be used with docker project [ubuntu-jboss-gmlc](http://github.com/masood-alam/ubuntu-jboss-gmlc).

Or this zip file can be extracted in root folder and run as standalone application.


*Running as Standalone Application*
-----------------------------------
unzip the archive file

~$unzip gmlc/release/jboss-5.1.0.GA-nw.zip

run bin/run.sh script

visit http://localhost:8080/jss7-mangamgent-console in the Browser
configure sctp, mtp3, sccp stack parameters
 