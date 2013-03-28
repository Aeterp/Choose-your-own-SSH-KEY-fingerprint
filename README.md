Choose-your-own-SSH-KEY-fingerprint
===================================

Application uses OpenSSL to generate an SSH KEY pair having the key fingerprints you specify. 

Requires OpenSSL be installed on your FreeBSD/Linux machine. Application was developed under FreeBSD but
works on Linux too. Point the application to where the BASH interpreter is located on your server
if it is not installed at /usr/local/bin/bash (FreeBSD).

As an example, I wanted an all numberic key (no letters a-f), so
the program generated 81:52:10:83:57:72:24:23:51:96:22:58:79:12:30:16 and this is my key fingerprint.

These are intended for servers because many people see the host's key fingerprint when they connect for
the first time but these work for for anybody.

There is a limit to what can be done with the digits 0-9 and A-F but that limitation aside there is
plenty of interesting fingerprints to have.

Like: 8B:AD:F0:0D...  (Ate Bad Food) OR

      FA:CE:B0:OC...  (FACEBOOK)
