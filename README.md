#LogRotator#
LogRotator will free disk resources automatically for you, it resides as windows service and primarily does two things.
 
* Compress log, xls or any other files to increase space, they can be extracted with any zip archive handler.
* Delete files older than specific duration, based on last modified timestamp
 
##How to Configure##
It works on LogRotator.xml configuration file, pretty much all tags are self-explanatory, you will find details about each tag in the configuration file. Configuration through UI is under development. 
 
##Ideal Configuration##
Offset duration for compressing any log files should be more than 2 to 3 days so that it would be easier for developers to send their reports or logs without the need for decompression.
 
##Install/Uninstall##
Simply run Install.bat file to install this service, and UnInstall.bat to uninstall from host machine. Service is set to run automatically in host restart. Remember service will run from the same folder where you ran Install.bat, so extracts files in the appropriate folder first.
 
##LogRotator Logs##
LogRotator also generates its own logs therefore you will find two configurations (as can be seen from above config) related two to LogRotator service, it will automatically compress logs generated by this services after two days and delete it after seven days, before careful when changing or adding new log/report folders.
 
##Requirement##
It requires .NET 4.0 Extended Profile to be installed on host machine.

##Warranty##
This service comes on as is bases, with warranty to work flawlessly.