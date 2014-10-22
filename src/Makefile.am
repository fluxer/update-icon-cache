bin_PROGRAMS = update-icon-cache
update_icon_cache_SOURCES = updateiconcache.c
update_icon_cache_CFLAGS = $(GLIB_CFLAGS) $(GLIB_LIBS) $(GDK_CFLAGS) $(GDK_LIBS)

EXTRA_DIST = gtkiconcachevalidator.c gtkiconcachevalidator.h

install-exec-hook:
	ln -s update-icon-cache $(DESTDIR)$(bindir)/gtk-update-icon-cache