=================================================
Enabling Supervisord support
=================================================

:Homepage:  https://pypi.python.org/pypi/supervisor/
:Credits:   Copyright © 1990-2014, Python Software Foundation
:Licence:   Python License


REQUIREMENTS
============

- Python 2.6
- Python-Devels 2.6
- https://pypi.python.org/pypi/supervisor


INSTALL
=======
pip install supervisor 

copy supervisord.conf under /etc & copy supervisord-init under /etc/init.d/supervisord

chmod ug+x /etc/init.d/supervisord && chkconfig supervisord on

 ( plz don't install by Yum, the version is very old and buggy )


USAGE
=====
/etc/init.d/supervisord {start|stop|status|restart|reload|force-reload|condrestart}

/etc/init.d/supervisord start
(Starting supervisord:)
(ftp-cloudfs                   STARTING )

/etc/init.d/supervisord status
(ftp-cloudfs                     RUNNING    pid 9729, uptime 0:13:06)


supervisorctl stop ftp-cloudfs 
(ftp-cloudfs: stopped)

/etc/init.d/supervisord status
(ftp-cloudfs                              STOPPED    Apr 07 20:25 PM)
