dist_noinst_DATA =     \
	ipa.conf.in \
	ipaclient.conf.in

systemdtmpfiles_DATA =         \
	ipa.conf \
	ipaclient.conf

CLEANFILES = $(systemdtmpfiles_DATA)

%: %.in Makefile
	sed \
		-e 's|@HTTPD_GROUP[@]|$(HTTPD_GROUP)|g' \
		 '$(srcdir)/$@.in' >$@
