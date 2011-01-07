========================================
About
========================================
pc_xmpp_cpumon.py is a simple python script that runs a small GUI and sends your
CPU utilization percentage to the Exosite over XMPP.

License is BSD, Copyright 2010, Exosite LLC

Built/tested with Python 2.6.5

========================================
Quick Start
========================================
****************************************
1) install python
****************************************
http://www.python.org/download/
http://www.python.org/download/releases/2.6.5/
http://www.python.org/ftp/python/2.6.5/python-2.6.5.msi

****************************************
2) install xmpppy
****************************************
http://xmpppy.sourceforge.net/
http://sourceforge.net/projects/xmpppy/
http://sourceforge.net/projects/xmpppy/files/xmpppy/0.4.0/xmpppy-0.4.0.win32.exe/download

If running Debian Linux (or Ubuntu), you can > apt-get install python-xmpp

****************************************
3) install psutil
****************************************
--) download psutil and install (http://code.google.com/p/psutil/)
--) test by running python command prompt and typing "import psutil,time" and
    then "print psutil.cpu_times()"

If running Debian Linux (or Ubuntu), you can > apt-get install python-psutil
* Note, there is a bug in psutil versions earlier than 1.3.0 where it will not
  report correct cpu utilization.  Ubuntu may not have 1.3.0, so you have to 
  manually update the library (whereis pymodules...)

****************************************
4) install tk
****************************************
If running Debian Linux (or Ubuntu), you can > apt-get install python-tk

****************************************
5) test it out
****************************************
get python script "exompp_cpumon.py" and "options.cfg"
--) update the default credentials in options.cfg to use your xmpp login and 
    device CIK
--) run the script (> python exompp_cpumon.py)
--) verify the app connects, creates a datasource and sends data (no errors 
    should be generated)
--) log into one.exosite.com and verify the your cpu utilization is being
    sent

****************************************
6) tweak it
****************************************
--) could use some menu options maybe?

========================================
Release Notes
========================================
****************************************
0.1.0
****************************************
--) First release, binaries created for Windows, Linux
