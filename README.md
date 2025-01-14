Please - really tiny sudo replacement
=====================================

'Please' aims to be little sudo without bells and whistles.
Only pam authentication and executing command.

Name **please** fits into unix naming conventions.
Where we have daemon instead of background process.
We are killing processes, not closing processes.
Now we can please to run privileged process.


Examples
--------

Reboot system by unprivileged user:

    $ please reboot

To get a file listing of an unreadable directory:

    $ please ls /usr/local/protected

Run a root shell:

    $ please -


Installation on Debian / Ubuntu
-------------------------------
1. Install git, compiler and libpam-dev: __apt-get install git build-essential libpam0g-dev__
2. Clone repository: __git clone https://github.com/MagikBSD/please.git__
3. Build and install: __make && make install__
4. Install (and edit) pam rules: __cp pam.d/please.Debian /etc/pam.d/please__


Installation on Fedora
----------------------
1. Install git, compiler and pam-devel: __dnf install git gcc pam-devel__
2. Clone repository: __git clone https://github.com/MagikBSD/please.git__
3. Build and install: __make && make install__
4. Install (and edit) pam rules: __cp pam.d/please.Fedora /etc/pam.d/please__


Installation on openSUSE
------------------------
1. Install git, compiler and pam-devel: __zypper install git gcc make pam-devel__
2. Clone repository: __git clone https://github.com/MagikBSD/please.git__
3. Build and install: __make && make install__
4. Install (and edit) pam rules: __cp pam.d/please.openSUSE /etc/pam.d/please__


Installation on FreeBSD
-----------------------
1. Install git: __pkg install git__ or __make install clean -C /usr/ports/devel/git__
2. Clone repository: __git clone https://github.com/MagikBSD/please.git__
3. Build and install: __make && make install__
4. Install (and edit) pam rules: __cp pam.d/please.FreeBSD /usr/local/etc/pam.d/please__
