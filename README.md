Choose-your-own-SSH-KEY-fingerprint
===================================

Application uses OpenSSL to generate SSH KEY pairs having a customized key fingerprint. This
applicationis intended to improve server security but the keys generated can be used for personal
protection too.

A tailor crafted SSH key fingerprint helps users protect against man in the middle attacks. MITM
attacks are often a crime of oppturtunity launched against all users on a downsteam network
connecting via SSH. Users connect to a wide variety of different servers. An attacker provides
the same SSH fingerprint to everybody.

When a organization has a policy that all their servers have SSH keys contain specific, easily
recognized pattern, e.g. ending in :88:88, 12:34, etc., then a fake fingerprint is easy to spot
because it doesn't contain the correct pattern. Users know right away when a fingerprint can't be
one of the company's server.

This scheme doesn't protect against the case where one specific server is being attacked. In this
case, an attacker has the oppturtunity to create a matching fingerprint ahead of time. However,
this type of server specific MITM is rare. Most often a MITM is a machine in an upsteam ISP
intruding on all SSH connections coming through it, taking what they can find.

The number of patterns you can ask the program for are endless. Mining them does take time. It
is best to setup and leave the program run in the background. Shorten the search/patterns if not
enough keys are found; lengthen them when you getting too many.

Example pattern: All numeric (no A, B, C, D or F). This is the key fingerprint I use
on Github: 81:52:10:83:57:72:24:23:51:96:22:58:79:12:30:16.

Keys having 12 of the same character in it: e4:36:ee:ad:ef:c6:c9:e3:3b:de:ed:e8:e1:8e:ee:5b,
in this case the letter 'e'.

Then there are many humorous ones, keys which begin with, "8B:AD:F0:0D..." (ATE BAD FOOD)
or "FA:CE:BO:OC..." (Facebook), etc.

The application comes preconfigured with a bunch of search patterns. Add or remove them will.
The application was developed on FreeBSD but runs on Linux or any other *nix type platform.
One will have to adjust the locations of some of the executables, bash on FreeBSD is in
/usr/local/bin/ which is different from other Unix.

And of course, I welcome changes, improvements, comments.

Hope the application helps keep you secure.

Aeterp Pretea
