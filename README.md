krb5-1.10-3-srpm
================

SRPM building tools for krb5-1.10.3 for runing Samba 4 on RHEL 6.

This tool taken from the RHEL 6.4 release, without modification.
The set of tools need to be built and installed in the following order.

	krb5-1.10.3-srpm
	iniparser-3.1-srpm

	libtalloc-2.0.8-srpm
	libtdb-1.2.11-srpm
	libldb-1.1.15-srpm
	libtevent-0.9.17-srpm

	samba-4.0.3-srpm

The "make" command will do these steps.

	make build	# Build the package on the local OS
	make all	# Use "mock" to build the packages with the local
			# smaba4repo-6-x96_64 configuration, which needs.
	make install	# Actually install the RPM's in the designated
			# location for smaba4repo-6-x86_64


		Nico Kadel-Garcia <nkadel@gmail.com>