# srs_configuration_bundle
support "include directive" in srs "https://github.com/ossrs/srs" conf file

Add function configuration bundle to init.d command of srs service
The function read conf fileand detect include directive in conf file like as format of nginx
It will create a new configuration file with name <confName>-bundle.conf in the same folder with configuration file and using this file for srs process. If no any include directive in configuration, the script is ignored
  
Tested in release 2.0.x

## How To Use
Just replace this file to original srs file at /etc/init.d/srs
Support build bundle configuration in start/restart/reload command
