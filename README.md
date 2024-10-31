This repo contains a moduler NxLog configs for both NxLog Community Eddition and NxLog Enterprise Edition. 
Does not work with NxLog manager!!

After installing rename the default nxlog.conf to something that will not be recognized as a config file. nxlog.orig is a good example of this.
The origional config file wil be located in one of the following directories below depending on the Operating System.
Windows file path is C:\Program Files\nxlog\conf
Linux file path is /opt/nxlog/etc/
Mac file path is  /opt/nxlog/etc/

Once the origional configuration file has been renamed, copy the new master configuration file to the same directory.
The new file located in this repository is NxLog-Globalconfig.conf. Once copied, rename the file to nxlog.conf
At the time of the writing of this, only the windows master config file has been written.

Now that the master config file has been written, the sub modules can be added to the /nxlog.d directory and will be picked up 
and run as a seperate module for each config file. 

If there are any issues with the config files, the logs will indicate which config has issues and can be easily fixed.
When a single config has issues, it does not stop the remaining configuration files from running.
