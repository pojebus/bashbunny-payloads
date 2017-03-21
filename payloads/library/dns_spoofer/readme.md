dns_spoofer
===========

Author: Michal Wysocki

Version: 1.0

Description
===========

Redirects HTTP traffic to Apache2 server running on Bunny. It works on
assumption that BashBunny adapter takes precedence  over host adapter. I have
noticed sometimes it won’t.

Configuration
=============

1.  Share your internet with Bunny in order to install Apache and dnsspoof -
    [see
    here](http://wiki.bashbunny.com/#!./index.md#Sharing_an_Internet_Connection_with_the_Bash_Bunny_from_Windows)

2.  Make sure that your repositories are up to date:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
apt-get update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1.  Install apache:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
apt-get install apache2
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1.  Install dnsspoof:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
apt-get install dsniff
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1.  Edit hosts file, by default it redirects all the HTTP traffic to local
    Apache

STATUS
======

| LED              | Status                              |
|------------------|-------------------------------------|
| Green (blinking) | Starting Apache (be patient)        |
| Blue             | Starting dnsspoof and ready to roll |
