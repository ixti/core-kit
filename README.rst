===========================
core-kit
===========================
1.0-prime branch
---------------------------

Core-kit contains the core ebuilds for Funtoo Linux. It is designed to be a part of the Funtoo Linux kits system.

The ``1.0-prime`` branch of gnome-kit is the initial, stable curated branch of core ebuilds for Funtoo. By 'curated', we
mean that the overlay is a fork of a collection of ebuilds from Gentoo Linux that we have found particularly stable and
will be continuing to maintain.

The ``-prime`` suffix indicates that we consider this branch to be production-quality, enterprise class stability and
will be only incorporating bug fixes for specific issues and security backports. We will *not* be bumping versions of
ebuilds unless absolutely necessary and we have very strong belief that they will not negatively impact the
functionality on anyone's system.

Based on these policies, you should consider ``1.0-prime`` to be a reference implementation of core packages for Funtoo
Linux that you can rely on to be stable and perform consistently over an extended period of time.

--------------------
Security Workarounds
--------------------

- ``net-dns/avahi`` has a not-yet-fixed vulnerability -- CVE-2017-6519 -- affecting versions 0.7 (latest version) and
  earlier.  Since no fix is currently available from the author, it is highly recommended that UDP multicast DNS traffic
  destined for port 5353 is blocked by a firewall, or that avahi is configured to not listen on externally-connected
  interfaces. See https://github.com/lathiat/avahi/issues/145

--------------
Security Fixes
--------------

January 24, 2018
~~~~~~~~~~~~~~~~

- ``sys-libs/glibc`` updated to 2.23-r6 to address CVE-2017-16997.


January 22, 2018
~~~~~~~~~~~~~~~~

- ``sys-devel/binutils`` has been updated to 2.29.1 to address CVE-2017-12456, CVE-2017-12799, CVE-2017-12967, CVE-2017-14128, CVE-2017-14129, CVE-2017-14130, CVE-2017-14333, CVE-2017-15023,
  CVE-2017-15938, CVE-2017-15939, CVE-2017-15996, CVE-2017-7209, CVE-2017-7210, CVE-2017-7223, CVE-2017-7224, CVE-2017-7225, CVE-2017-7227, CVE-2017-9743, CVE-2017-9746, CVE-2017-9749, CVE-2017-9750, CVE-2017-9751, CVE-2017-9755 and CVE-2017-9756.

January 13, 2018
~~~~~~~~~~~~~~~~

- ``dev-libs/libxml2`` has been updated to 2.9.7-r1 to address CVE-2017-16392, CVE-2017-16391, CVE-2017-9049 and CVE-2017-8872.

January 2, 2018
~~~~~~~~~~~~~~~

- ``net-wireless/hostapd`` has been updated to 2.4-r2 to address CVE-2015-1863, CVE-2015-4141, CVE-2015-4142, CVE-2015-8041, CVE-2015-5314, CVE-2015-5316
  CVE-2016-4476, CVE-2017-13077, CVE-2017-13078, CVE-2017-13079, CVE-2017-13080, CVE-2017-13081, CVE-2017-13082, CVE-2017-13086, CVE-2017-13087 and CVE-2017-13088.

December 28, 2017
~~~~~~~~~~~~~~~~~

- ``app-admin/sudo`` has been updated to 1.8.21_p2 to address CVE-2017-1000368 (CVE-2017-1000367 was already addresssed via patch.)

December 21, 2017
~~~~~~~~~~~~~~~~~
- ``dev-libs/openssl`` has been updated to 1.0.2n to address CVE-2017-3735, CVE-2017-3736, CVE-2017-3737 and CVE-2017-3738.

December 18, 2017
~~~~~~~~~~~~~~~~~

- ``net-misc/rsync`` has been udpated to 3.1.2-r1 to address CVE-2017-16548, CVE-2017-17433 and CVE-2017-17434.

September 15, 2017
~~~~~~~~~~~~~~~~~~

- ``net-wireless/bluez`` was updated to 5.44-r1 to address CVE-2017-1000250 (blueborne vulnerability.)

---------------
Reporting Bugs
---------------

To report bugs or suggest improvements to core-kit, please use the Funtoo Linux bug tracker at https://bugs.funtoo.org.
Thank you! :)
