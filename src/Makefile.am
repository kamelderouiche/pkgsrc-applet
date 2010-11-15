


AM_CPPFLAGS = \
	-DPACKAGE_LOCALE_DIR=\""$(prefix)/$(DATADIRNAME)/locale"\" \
	-DPACKAGE_SRC_DIR=\""$(srcdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(datadir)"\" \
	$(PKGSRC_APPLET_CFLAGS)


bin_PROGRAMS = pkgsrc-applet

pkgsrc_applet_SOURCES = \
	 main.py 	\
	__init__.py		

pkgsrc_applet_LDFLAGS = \
	-Wl,--export-dynamic


